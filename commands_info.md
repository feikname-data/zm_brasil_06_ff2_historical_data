## Commands information
  This file contains information about each console command available for the
"ZM BRASIL #06 (FF2)" Team Fortress 2 server.

**THIS FILE UNDER CONSTRUCTION.**

Please note that FF2 is the sucessor of VSH.

Currently explained:
 * [`amp`, `amplifier`]
 * [`amp_help`]
 * [`em`, `equip`, `equipmodels`, `mm`, `tf_models`]

To be explained in detail:
 * [`ff`] - Show friendly fire status
 * [`ff2`, `hale`] - Freak Fortress 2 general menu
 * [`ff2_classinfo`, `ff2classinfo`, `hale_classinfo`, `haleclassinfo`] - Display information about your class powers
 * [`ff2_hp`, `ff2hp`, `hale_hp`, `halehp`] - Show the boss hp to everyone
 * [`ff2_music`, `ff2music`, `hale_music`, `halemusic`] - Show the boss music options menu
 * [`ff2_new`, `ff2new`, `hale_new`, `halenew`] - Display the FF2 plugin changelog and check for updates
 * [`ff2_next`, `ff2next`, `hale_next`, `halenext`] - See who's going to be the next hale
 * [`ff2_resetpoints`, `ff2resetpoints`, `hale_resetpoints`, `haleresetpoints`] - Reset your queue points
 * [`ff2_voice`, `ff2voice`, `hale_voice`, `halevoice`] - Toggle boss voice sounds
 * [`ff2_boss`, `ff2boss`, `hale_boss`, `haleboss`] - Set your boss (VIP only)
 * [`ff2dmg`, `haledmg`] - Display the top damage scoreboard of each round in the left superior corner
 * [`ff2toggle`, `haletoggle`] - Toggle if you want to be hale or not (may not work if there are few players or many people with this options enabeld too)
 * [`fp`, `sm_fp`, `sm_firstperson`] - Set your view to first person
 * [`tp`, `sm_tp`, `sm_thirdperson`] - Set your view to third person
 * [`goomba_off`] - Disable stomps for yourself. As of July 2017, due to a bug report of mine, it can no longer be exploited
 * [`listmaps`] - Output the map cycle to the console
 * [`motd`] - Opens the *m*essage *o*f *t*he *d*ay
 * [`nextmap`] - Shows the map that will be loaded after the round ends
 * [`sm_bet`] - Allows you to bet credits on either red or blu
 * [`sm_browse`] - Opens the Steam built-in [CEF] browser inside the motd page to the chosen URL
 * [`sm_buildinghats`] - Toggles if your engineer constructions will have hats. I did not test if it works with rtd and amp
 *

Commands listed in the help text that **DO NOT** work:
```text
gameme_browse
gameme_csay
gameme_hint
gameme_khint
gameme_message_prefix_clear
gameme_msay
gameme_player_action
gameme_psay
gameme_raw_message
gameme_redirect
gameme_swap
gameme_team_action
gameme_tsay
gameme_world_action
sm_advertisements_reload
```

Missing commands to explain at least basically:
```text
sm_colorize_colors
sm_cookies
sm_credits
sm_drop
sm_dsp
sm_gift
sm_givecredits
sm_help
sm_inv
sm_irs_kicklist_reload
sm_ks
sm_me
sm_mirror
sm_music
sm_musicfull
sm_musicstop
sm_musicto
sm_musicyt
sm_nominate
sm_offer
sm_particles
sm_radiooff
sm_rerollhat
sm_resetplayer
sm_revote
sm_rtv
sm_searchcmd
sm_settings
sm_store
sm_store_custom_credits
sm_trade
sm_vip
sm_voicefx
sm_yt
sm_yt_full
sm_yt_stop
sm_yt_to
tauntcrits_help
tauntcrits_info
tf2items_disable
tf2items_enable
timeleft
voicemenu
```

### [`amp`, `amplifier`]
This command is part of the [The Amplifier](https://forums.alliedmods.net/showthread.php?p=1179897) plugin.

It brings up a menu for selecting which building the engineer will use, and it can be either:
 * The tf2 traditional dispenser; or
 * The amplifier, which grants crits within a radious specified by the server to teammates and enemy spies. It cannot be upgraded.

  Selecting the amplifier as your building is not recommend, because crits can be
awarded for 30 seconds simply by taunting, thus making the dispenser far more useful.

  The server might output `Unknown command: amp` to the console, but it works anyway.
Also, the menu will only show if you're currently an engineer, thus, you might
need to wait your respawn if you just switched classes.

### [`amp_help`]
This command is part of [The Amplifier](https://forums.alliedmods.net/showthread.php?p=1179897) plugin.

  Displays a pt-br translated text about what `amp` does. It is hard to understand
and badly translated. If you need info about the `amp` command, read the [`amp`, `amplifier`] entry above.

The server might output `Unknown command: amp_help` to the console, but it works anyway.

### [`em`, `equip`, `mm`, `equipmodels`, `tf_models`]
This command is part of the [Model Manager](https://forums.alliedmods.net/showthread.php?t=164630) plugin.

It brings up the model selection menu (think of models as alternate skins).

  Only some people have one or more skins available for them currently, so it is
useless for most players.

Known players bearing at least one model:
 * The Doge Master (claims to have received one as an award for helping the server)
