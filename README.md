## ZM BRASIL #06 (FF2) - Historical data
  This repository contains historical data of the "ZM BRASIL #06 (FF2)" Team
Fortress 2 server.

  The intention is to do bug reports in case anything goes missing or to simply analyze
how the server has been changing over time.

## Directory structure
  I collect the `sm`, `sm_help` (all pages), and `sm plugins` (all pages) commands
console output and put each one in a different file formatted as `zm_06_ff2_COMMANDTYPE_YEAR_MONTH_DAY.txt`
(e.g. `zm_06_ff2_help_output_2017_05_20.txt`) inside the `gathered_data` folder.

 * `COMMANDTYPE` field may be `plugins`, `help_output`, or `sm_output`.
 * `YEAR` Year number (in [Common Era](https://en.wikipedia.org/wiki/Common_Era)), with 4 digits.
 * `MONTH` Month of the year, with 2 digits and leading zeroes if necessary.
 * `DAY`: Day of the month with, 2 digits and leading zeroes if necessary.

  You may view the data separately by browsing the `gathered_data` directory or
you may browse the [`zm_06_ff2_help_output_for_diff_view.txt` history](https://github.com/feikname-data/zm_brasil_06_ff2_historical_data/commits/master/zm_06_ff2_help_output_for_diff_view.txt)
and the [`zm_06_ff2_plugins_for_diff_view.txt` history](https://github.com/feikname-data/zm_brasil_06_ff2_historical_data/commits/master/zm_06_ff2_plugins_for_diff_view.txt)
for a convenient diff view.

## How is the data updated?
  The data is updated by me joining the server, typing the `sm`, `sm_help`, and
`sm plugins` commands into the console and then sorting the output of each command
into files inside the `gathered_data` directory.

  To sort the output, I use [Notepad++](https://notepad-plus-plus.org/) to trim
any trailing spaces and [lexicographically](https://en.wikipedia.org/wiki/Lexicographical_order)
sort each line.

I use some regexes to make the job easier too:

For `sm_help`:
 * `^(?!\[[0-9][0-9][0-9]\]).*` to remove all lines that do NOT start with `[###]`, where ### are numbers (e.g. RTD and chat messages noise from `console.log`)
 * `\[[0-9][0-9][0-9]\] ` to remove all `[###] ` prefixes after it, so the diff can focus only in the removal and addition of items, instead of their ordering.

For `sm plugins`:
 * `^(?! ").*` to remove all lines that do NOT start with ` "` (e.g. RTD and chat messages noise from `console.log`)

For both:
 * `^(.*?)$\s+?^(?=.*^\1$)` to remove duplicate entries next to each other (requires sorting first, to ensure it works as intended).

For `commands_info.md`
 * `^(.*)$` replaced with ` * \1` to make the list
