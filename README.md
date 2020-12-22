# CSGO MFT Dedicated Server

## This Project Currently Contains The Following Addons/Plugins:

* __SourceMod v1.10.0__, Can be found [here](https://www.sourcemod.net)
* __Metamod: Source v1.11.0__, Can Be found [here](http://www.metamodsource.net)
* __Fortnite Emotes Extended version v1.4.2__, Located and Documented in this [thread](https://forums.alliedmods.net/showthread.php?t=318981)
* __Gloves v1.0.5__, Located and Documented in this [thread](https://forums.alliedmods.net/showthread.php?t=299977)
* __Weapons v1.7.1__, Located and Documented in this [thread](https://forums.alliedmods.net/showthread.php?t=298770)
* __PTaH-V1.1.3-build19__, Can be found [here](https://ptah.zizt.ru)
* __RankMe Kento Edition v3.0.3.Kento.33.2__, Located and Documented in this [thread](https://forums.alliedmods.net/showthread.php?t=290063)
* __Matchmaking Ranks by Points__, Can be found [here](https://github.com/luis-rei97/MatchMaking-Ranks-By-Points)
* __Move Commands v2.0.0__, Located and Documented in this [thread](https://forums.alliedmods.net/showthread.php?p=2041122)
* __Pug Setup v2.0.5__, Located and Documented in this [thread](https://forums.alliedmods.net/showthread.php?t=244114)
* __Advertisements v2.0__, Located and Documented in This [thread](https://forums.alliedmods.net/showthread.php?t=155705)
* __eItems v0.10__, Can Be Found [here](https://github.com/quasemago/eItems)
* __Rest In Pawn Extension v1.2.1__, Located And Documented in This [thread](https://forums.alliedmods.net/showthread.php?t=298024)
* __Multi-Colors__, Can be found [here](https://github.com/Bara/Multi-Colors)
* __Weapon Stickers v1.0.13__, Located And Documented in this [thread](https://forums.alliedmods.net/showthread.php?t=327078)


# CVar's and in-game Commands

## * Fortnite Emotes
> You can modify the CVars below in cfg/sourcemod/fortnite_emotes_extended.cfg file
### ConVars
```
// admin flag for !emotes command (empty for all players)
// -
// Default: ""
sm_emotes_admin_flag_menu ""

// Cooldown for emotes in seconds. -1 or 0 = no cooldown.
// -
// Default: "4.0"
sm_emotes_cooldown "4.0"

// Sound volume for the emotes.
// -
// Default: "0.4"
sm_emotes_soundvolume "0.4"

// Hide enemy players when dancing
// -
// Default: "0"
// Minimum: "0.000000"
// Maximum: "1.000000"
sm_emotes_hide_enemies "0"

// Hide weapons when dancing
// -
// Default: "1"
// Minimum: "0.000000"
// Maximum: "1.000000"
sm_emotes_hide_weapons "1"

// Enable/Disable sounds for emotes.
// -
// Default: "1"
// Minimum: "0.000000"
// Maximum: "1.000000"
sm_emotes_sounds "1"

// Teleport back to the exact position when he started to dance. (Some maps need this for teleport triggers)
// -
// Default: "0"
// Minimum: "0.000000"
// Maximum: "1.000000"
sm_emotes_teleportonend "1"
```
### Commands
```
//Commands:
//sm_emotes - user command for main menu.
//sm_setemotes <#userid|name> <emote ID> , (emote ID from 1 to 84) - ADMIN COMMAND.
```

## * Gloves
> You can modify the CVars below in cfg/sourcemod/gloves.cfg file
### ConVars
´´´
sm_gloves_db_connection - Database connection name in databases.cfg to use
Default: "storage-local"

sm_gloves_table_prefix - Prefix for database table (example: "xyz_")
Default: ""

sm_gloves_chat_prefix - Prefix for chat messages Currently there are no messages shown anyway.
Default: "[oyunhost.net]"

sm_gloves_enable_float - Enable/Disable gloves float options
Default: "1"

sm_gloves_float_increment_size - Increase/Decrease by value for gloves float
Default: "0.2"

sm_gloves_enable_world_model - Enable/Disable gloves to be seen by other living players
Default: "1"
´´´
### Commands
```

```

## * Weapons & Knives
>You can modify the CVars below in cfg/sourcemod/weapons.cfg file
### ConVars
```
sm_weapons_db_connection - Database connection name in databases.cfg to use
Default: "storage-local"

sm_weapons_table_prefix - Prefix for database table (example: "xyz_")
Default: ""

sm_weapons_chat_prefix - Prefix for chat messages
Default: "[oyunhost.net]"

sm_weapons_knife_stattrak_mode - 0: All knives show the same StatTrak counter (total knife kills) 1: Each type of knife shows its own separate StatTrak counter
Default: "0"

sm_weapons_enable_float - Enable/Disable weapon float options
Default: "1"

sm_weapons_enable_nametag - Enable/Disable name tag options
Default: "1"

sm_weapons_enable_stattrak - Enable/Disable StatTrak options
Default: "1"

sm_weapons_enable_seed - Enable/Disable skin seed options
Default: "1"

sm_weapons_float_increment_size - Increase/Decrease by value for weapon float
Default: "0.05"

sm_weapons_enable_overwrite - Enable/Disable players overwriting other players' weapons (picked up from the ground) by using !ws command
Default: "1"

sm_weapons_grace_period - Grace period in terms of seconds counted after round start for allowing the use of !ws command. 0 means no restrictions
Default: "0"

sm_weapons_inactive_days - Number of days before a player (SteamID) is marked as inactive and his data is deleted. (0 or any negative value to disable deleting)
Default: "30"
```
### Commands
```

```


* ##  RankMe Kento Edition
>You can modify the CVars below in csgo\cfg\sourcemod\kento.rankme.cfg
### ConVars
```
rankme_enabled    "1"    //Is RankMe enabled? 1 = true 0 = false"
rankme_rankbots    "0"    //Rank bots? 1 = true 0 = false"
rankme_autopurge    "0"    //Auto-Purge inactive players? X = Days  0 = Off"
rankme_points_bomb_defused_team     "2"    //How many points CTs got for defusing the C4?"
rankme_points_bomb_defused_player     "2"    //How many points the CT who defused got additional?"
rankme_points_bomb_planted_team     "2"    //How many points TRs got for planting the C4?"
rankme_points_bomb_planted_player     "2"    //How many points the TR who planted got additional?
rankme_points_bomb_exploded_team     "2"    //How many points TRs got for exploding the C4?
rankme_points_bomb_exploded_player     "2"    //How many points the TR who planted got additional?
rankme_points_hostage_rescued_team     "2"    //How many points CTs got for rescuing the hostage?
rankme_points_hostage_rescued_player     "2"    //How many points the CT who rescued got additional?
rankme_points_hs    "1"    //How many additional points a player got for a HeadShot?
rankme_points_kill_ct     "2"    //How many points a CT got for killing?
rankme_points_kill_tr     "2"    //How many points a TR got for killing?
rankme_points_kill_bonus_ct    "1"    //How many points a CT got for killing additional by the diffrence of points?
rankme_points_kill_bonus_tr    "1"    //How many points a TR got for killing additional by the diffrence of points?
rankme_points_kill_bonus_dif_ct     "100"    //How many points of diffrence is needed for a CT to got the bonus?
rankme_points_kill_bonus_dif_tr     "100"    //How many points of diffrence is needed for a TR to got the bonus?
rankme_points_ct_round_win     "0"    //How many points CT got for winning the round?
rankme_points_tr_round_win     "0"    //How many points TR got for winning the round?
rankme_points_ct_round_lose    "0"    //How many points CT lost for losing the round?
rankme_points_tr_round_lose    "0"    //How many points TR lost for losing the round?
rankme_points_knife_multiplier     "2.0"    //Multiplier of points by knife
rankme_points_taser_multiplier     "2.0"    //Multiplier of points by taser
rankme_points_start     "1000"    //Starting points
rankme_minimal_kills     "0"    //Minimal kills for entering the rank
rankme_percent_points_lose     "1.0"    //Multiplier of losing points. (WARNING: MAKE SURE TO INPUT IT AS FLOAT) 1.0 equals lose same amount as won by the killer, 0.0 equals no lose
rankme_points_lose_round_ceil    "1"    //If the points is f1oat, round it to next the highest or lowest? 1 = highest 0 = lowest
rankme_changes_chat    "1"    //Show points changes on chat? 1 = true 0 = false
rankme_show_rank_all     "0"    //When rank command is used, show for all the rank of the player? 1 = true 0 = false
rankme_rank_all_timer     "30.0"    //Cooldown timer to prevent rank command spam. 0.0 = disabled
rankme_show_bots_on_rank     "0"    //Show bots on rank/top/etc? 1 = true 0 = false
rankme_resetownrank     "0"    //Allow player to reset his own rank? 1 = true 0 = false
rankme_minimumplayers     "2"    //Minimum players to start giving points
rankme_vip_enabled     "0"    //Show AS_ maps statiscs (VIP mod) on statsme and session?
rankme_points_vip_escaped_team     "2"    //How many points CTs got helping the VIP to escaping?
rankme_points_vip_escaped_player     "2"    //How many points the VIP got for escaping?
rankme_points_vip_killed_team     "2"    //How many points TRs got for killing the VIP?
rankme_points_vip_killed_player     "2"    //How many points the TR who killed the VIP got additional?
rankme_points_lose_tk     "0"    //How many points a player lose for Team Killing?
rankme_points_lose_suicide     "0"    //How many points a player lose for Suiciding?
rankme_rank_by     "0"    //Rank players by? 0 = STEAM:ID 1 = Name 2 = IP
rankme_ffa     "0"    //Free-For-All (FFA) mode? 1 = true 0 = false
rankme_mysql     "0"    //Using MySQL? 1 = true 0 = false (SQLite)
rankme_dump_db     "0"    //Dump the Database to SQL file? (required to be 1 if using the web interface and SQLite, case MySQL, it won't be dumped) 1 = true 0 = false
rankme_gather_stats    "1"    //Gather Statistics (a.k.a count points)? (turning this off won't disallow to see the stats already gathered) 1 = true 0 = false
rankme_days_to_not_show_on_rank     "0"    //Days inactive to not be shown on rank? X = days 0 = off
rankme_rank_mode    "1"    //Rank by what? 1 = by points 2 = by KDR
rankme_sql_table    "rankme"    //The name of the table that will be used. (Max: 100)
rankme_chat_triggers    "1"    //Enable (non-command) chat triggers. (e.g: rank, statsme, top) Recommended to be set to 0 when running with EventScripts for avoiding double responses. 1 = true 0 = false
rankme_points_mvp_ct    "1"    //How many points a CT got for being the MVP?
rankme_points_mvp_tr    "1"    //How many points a TR got for being the MVP?
rankme_points_bomb_pickup     "0"    //How many points a player gets for picking up the bomb?
rankme_points_bomb_dropped    "0"    //How many points a player loess for dropping the bomb?
rankme_points_assiist_kill    "1"    //How many points a player gets for assist kill?
ankme_points_match_win    "2"    //How many points a player win for winning the match?
rankme_points_match_lose    "2"    //How many points a player loess for losing the match?
rankme_points_match_draw    "0"    //How many points a player win when match draw?"
rankme_announcer_player_connect    "1"    //Announce when a player connect with position and points?
rankme_announcer_player_connect_chat    "1"    //Announce when a player connect at chat?
rankme_announcer_player_connect_hint    "0"    //Announce when a player connect at hintbox?
rankme_announcer_player_disconnect    "1"    //Announce when a player disconnect with position and points?
rankme_announcer_top_player_connect    "1"    //Announce when a top player connect?
rankme_announcer_top_pos_player_connect    "10"    //Max position to announce that a top player connect?
rankme_announcer_top_player_connect_chat    "1"    //Announce when a top player connect at chat?
rankme_announcer_top_player_connect_hint    "0"    //Announce when a top player connect at hintbox?
rankme_gather_stats_warmup "1" //Gather Statistics In Warmup?
rankme_points_min_enabled "1" // Is minimum points enabled? 1 = true 0 = false
rankme_points_min "0" // Minimum points
rankme_rank_cache "1" //Get player rank via cache, auto build cache on every OnMapStart.
rankme_points_ns    "1"    //How many additional points a player got for a no scope kill?
rankme_points_ns_allsnipers    "0"    //0: ssg08 and awp only, 1: ssg08, awp, g3sg1, scar20
rankme_points_fb    "1"    //How many additional points a player got for a First Blood?
rankme_points_blind  "1"  // How many additional points a player got for a flashed kill?
rankme_points_smoke  "1"  // How many additional points a player got for killing through smoke?
rankme_points_lose_atk  "1" // How many points a player lose for Assist Team Killing?
rankme_points_assiist_flash  "1"  // How many points a player gets for assist flash kill?
rankme_points_lose_atf  "1"  // How many points a lose for team assist flash kill?
rankme_points_wall  "1"  // How many additional points a player got for wallbang? 
```
### Commands
```
//Admin Commands
sm_resetrank //RankMe: Resets the rank of a player
sm_rankme_remove_duplicate //RankMe: Removes the duplicated rows on the database
sm_rankpurge //RankMe: Purges from the rank players that didn't connected for X days
sm_resetrank_all //RankMe: Resets the rank of all players

//Player Commands
sm_session //RankMe: Shows the stats of your current session
sm_rank //RankMe: Shows your rank
sm_top //RankMe: Shows the TOP
sm_topweapon //RankMe: Shows the TOP ordered by kills with a specific weapon
sm_topacc //RankMe: Shows the TOP ordered by accuracy
sm_tophs //RankMe: Shows the TOP ordered by HeadShots
sm_toptime //RankMe: Shows the TOP ordered by Connected Time
sm_topkills //RankMe: Shows the TOP ordered by kills
sm_topdeaths //RankMe: Shows the TOP ordered by deaths
sm_hitboxme //RankMe: Shows the HitBox stats
sm_weaponme //RankMe: Shows the kills with each weapon
sm_resetmyrank //RankMe: Resets your own rank
sm_statsme //RankMe: Shows your stats
sm_next //RankMe: Shows the next 9 players above you on the TOP
sm_statsme2 //RankMe: Shows the stats from a player
sm_rankme //RankMe: Shows a menu with the basic commands
sm_topassists //RankMe: Shows the TOP ordered by Assists
sm_toptk //RankMe: Shows the TOP ordered by TKs
sm_topmvp //RankMe: Shows the TOP ordered by MVPs
sm_topdamage //RankMe: Shows the TOP ordered by damage
sm_rankmechat //Disable rankme chat messages
sm_topkdr // RankMe: Shows the TOP ordered by kdr
sm_toppoints // RankMe: Shows the TOP ordered by points
sm_topfb // RankMe: Shows the TOP ordered by first bloods
sm_topns // RankMe: Shows the TOP ordered by no scopes
sm_topnsd // RankMe: Shows the TOP ordered by no scope distance
sm_topfk // RankMe: Shows the TOP ordered by flashed kills
sm_topthrusmoke // RankMe: Shows the TOP ordered by killing through smokes
sm_topwall // RankMe: Shows the TOP ordered by wallbangs 
```

## * MatchMaking Ranks By Points
> You can modify the CVars below in cfg\sourcemod\ranks_matchmaking.cfg
### ConVars
```
ranks_matchmaking_typeofrank (Default: 0) - Type of Rank that you want to use for this plugin (0 for Kento Rankme, 1 for GameMe, 2 for ZR Rank, 3 for HLStatsX)
ranks_matchmaking_prefix (Default: "[{purple}Fake Ranks{default}]") - Chat Prefix
ranks_matchmaking_flag (Default: 0) - Flag to restrict the ranks to certain players (0 enable the ranks for everyone)
ranks_matchmaking_point_s1 (Default: 100) - Number of Points to reach Silver I
ranks_matchmaking_point_s2 (Default: 150) - Number of Points to reach Silver II
ranks_matchmaking_point_s3 (Default: 200) - Number of Points to reach Silver III
ranks_matchmaking_point_s4 (Default: 300) - Number of Points to reach Silver IV
ranks_matchmaking_point_se (Default: 400) - Number of Points to reach Silver Elite
ranks_matchmaking_point_sem (Default: 500) - Number of Points to reach Silver Elite Master
ranks_matchmaking_point_g1 (Default: 600) - Number of Points to reach Gold Nova I
ranks_matchmaking_point_g2 (Default: 750) - Number of Points to reach Gold Nova II
ranks_matchmaking_point_g3 (Default: 900) - Number of Points to reach Gold Nova III
ranks_matchmaking_point_g4 (Default: 1050) - Number of Points to reach Gold Nova IV
ranks_matchmaking_point_mg1 (Default: 1200) - Number of Points to reach Master Guardian I
ranks_matchmaking_point_mg2 (Default: 1400) - Number of Points to reach Master Guardian II
ranks_matchmaking_point_mge (Default: 1600) - Number of Points to reach Master Guardian Elite
ranks_matchmaking_point_dmg (Default: 1800) - Number of Points to reach Distinguished Master Guardian
ranks_matchmaking_point_le (Default: 2000) - Number of Points to reach Legendary Eagle
ranks_matchmaking_point_lem (Default: 2200) - Number of Points to reach Legendary Eagle Master
ranks_matchmaking_point_smfc (Default: 2400) - Number of Points to reach Supreme Master First Class
ranks_matchmaking_point_ge (Default: 2700) - Number of Points to reach Global Elite
ranks_matchmaking_hudoverlay (Default: 1) -> Chooses between a HUD Text Message (0) or an Overlay (1). Overlays are made by RoadSide Romeo;
ranks_matchmaking_soundenable (Default: 1) -> Enable sounds when a player ranks up or deranks;
ranks_matchmaking_soundrankup (Default: "levels_ranks/levelup.mp3") -> Path to the sound which will play on Rank Up (needs ranks_matchmaking_soundenable set to 1);
ranks_matchmaking_soundrankdown (Default: "levels_ranks/leveldown.mp3") -> Path to the sound which will play on Derank (needs ranks_matchmaking_soundenable set to 1);
```

### Commands
```
sm_mm - It opens the Ranks Menu, with the option to check the rank points;
```

## * Move Commands
>
### ConVars
```
movecommands_enable_adminmenu Enable / Disable MoveCommands in Adminmenu (Default: 1)
movecommands_enable_afk Enable / Disable AFK Command (Default: 1)
movecommands_enable_resetscore_command Enable / Disable ResetScore Command (Default: 0)
movecommands_enable_spec Enable / Disable Spec Command (Default: 1)
movecommands_enable_swap Enable / Disable Swap Command (Default: 1)
movecommands_enable_swapct Enable / Disable Swap CT Command (Default: 1)
movecommands_enable_swapt Enable / Disable Swap T Command (Default: 1)
movecommands_enable_fswap Enable / Disable Force Swap Command (Default: 1)
movecommands_enable_swaproundend Enable / Disable Swap Round End Command (Default: 1)
movecommands_enable_swapdeath Enable / Disable Swap Player Death Command (Default: 1)
movecommands_enable_exchangeteams Enable / Disable Exchange Teams Command (Default: 1)
movecommands_enable_swapallct Enable / Disable Swap All Players To CT Command (Default: 1)
movecommands_enable_swapallt Enable / Disable Swap All Players To T Command (Default: 1)
movecommands_enable_swapallspec Enable / Disable Swap All Players To Spec Command (Default: 1)

Enable/Disable Drops
movecommands_enable_drop_bomb Enable / Disable Bomb Drop (Default: 1)
movecommands_enable_drop_defuser Enable / Disable Defuser Drop (Default: 1)

ResetScore
movecommands_enable_resetscore Enable / Disable ResetScore after Swap/Spec Player (Default: 0)

TeamBalancer
movecommands_enable_teamabalancer Enable / Disable TeamBalancer
```

### Commands
```
sm_spec <Name/#UserID>
sm_swap <Name/#UserID>
sm_fswap <Name/#UserID>
sm_swaproundend <Name/#UserID>
sm_swapdeath <Name/#UserID>
sm_afk <Name/#UserID>
sm_exchange
sm_swapallct
sm_swapallt
sm_swapallspec
```

## * Pug Setup
> You can modify the CVars below in cfg\sourcemod\pugsetup\*.cfg
### ConVars
```
sm_pugsetup_admin_flag (default "b") - Admin flag to mark players as having elevated permissions
sm_pugsetup_announce_countdown_timer (default 1) - Whether to announce how long the countdown has left before the lo3 begins
sm_pugsetup_auto_randomize_captains (default 0) - When games are using captains, should they be automatically randomionce? Note you can still manually set them use .rand/!rand to redo the randomization
sm_pugsetup_autosetup (default 0) - Whether a pug is automatically setup using the default setup options or not
sm_pugsetup_autoupdate (default 1) - Whether the plugin may (if the Updater plugin is loaded) automatically update
sm_pugsetup_demo_name_format (default "pug_{TIME}_{MAP}") - Naming scheme for demos. You may use {MAP}, {TIME}, and {TEAMSIZE}. Make sure there are no spaces or colons in this
sm_pugsetup_exclude_spectators (default 0) - Whether to exclude spectators in the ready-up counts. Setting this to 1 will exclude specators from being selected captains as well.
sm_pugsetup_exec_default_game_config (default 1) - Whether gamemode_competitive (the matchmaking config) should be executed before the live config.
sm_pugsetup_force_defaults (default 0) - Whether the default setup options are forced as the setup options (note that admins can override them still).
sm_pugsetup_knife_cfg (default "sourcemod/pugsetup/knife.cfg") - Config to execute when the knife round begins. Cvars set in this file are automatically reverted to pre-knife-round values right before executing the live config.
sm_pugsetup_live_cfg (default "sourcemod/pugsetup/live.cfg") - Config to excute when the game goes live.
sm_pugsetup_maplist_aim_maps (default "aim_maps.txt") - If using aim map warmup, the maplist file in addons/sourcemod/configs/pugsetup to use. You may also use a workshop collection ID instead of a maplist you if you have the SteamWorks extension installed.
sm_pugsetup_maplist (default "maps.txt") - Maplist file in addons/sourcemod/configs/pugsetup to use. You may also use a workshop collection ID instead of a maplist you if you have the SteamWorks extension installed.
sm_pugsetup_mapvote_time (default 20) - How long the map vote should last if using map-votes.
sm_pugsetup_max_team_size (default 5) - Maximum size of a team when selecting teams.
sm_pugsetup_message_prefix (default "[{YELLOW}PugSetup{NORMAL}]" - The tag applied before plugin messages.
sm_pugsetup_money_on_warmup_spawn (default 0) - Whether clients recieve 16,000 dollars when they spawn. It's recommended you use mp_death_drop_gun 0 in your warmup config if you use this.
sm_pugsetup_mutual_unpausing (default 1) - Whether an unpause command requires someone from both teams to fully unpause the match.
sm_pugsetup_pausing_enabled (default 1) - Whether pausing is allowed.
sm_pugsetup_quick_restarts (default 0) - If set to 1, going live won't restart 3 times and will just do a single restart.
sm_pugsetup_setup_enabled (default 1) - Whether the sm_setup and sm_10man commands are enabled
sm_pugsetup_randomize_maps (default 1) - When maps are shown in the map vote/veto, whether their order is randomized.
sm_pugsetup_snake_captain_picks (default 0) - If set to 0: captains pick players in a ABABABAB order. If set to 1, in a ABBAABBA order. If set to 2, in a ABBABABA order.
sm_pugsetup_start_delay (default 5) - How many seconds before the lo3 process should being.
sm_pugsetup_time_format (default "%Y-%m-%d_%H%M") - Time format to use when creating demo file names.
sm_pugsetup_warmup_cfg (default "sourcemod/pugsetup/warmup.cfg") - Config file to run before/after games; should be in the csgo/cfg directory.
```

### Commands
```
.setup, begins the setup phase and sets the pug leader
.10man, an alias of setup with 5v5, captains, and a mapvote
.ready
.notready
.pause requests a pause (which takes effect next freezetime)
.unpause request an unpause
.start starts the game if auto-live has been disabled
.capt gives the pug leader a menu to select captains
.rand selects random captains
.leader gives a menu to change the game leader
.endgame force ends the game safely (only the leader can do this, note that this resets the leader to nobody)
.forceend force ends the game without a confirmation menu
.stay chooses to stay after winning a knife round
.swap chooses to swap after winning a knife round
.ct chooses to start on ct after winning a knife round
.t chooses to start on ct after winning a knife round

These are some helper commands for automation purposes the bypass requiring a player to press any menus:
sm_forceend (force ends the game with no confirmation menu)
sm_forcestart (force starts the match)

Other admin level commands are:
sm_addmap [temp|perm] to add a map to the maplist (defaults to permanently writing to the maplist)
sm_removemap [temp|perm] to remove a map from the maplist (defaults to permanently writing to the maplist)
sm_addalias to add a chat alias
sm_removealias to remove a chat alias
sm_setdefault to set a default setup menu setting
sm_setdisplay <0|1> to set whether a setup setting is displayed in the setup menu
```

## * Advertisements
>
### ConVars
```

```

### Commands
```
sm_advertisements_enabled (0/1, def 1)
Enable/disable displaying advertisements.

sm_advertisements_file (def "advertisements.txt")
File to read the advertisements from. Useful if you're running multiple servers from one installation, and want to use different advertisements per server.

sm_advertisements_interval (def 30)
Number of seconds between advertisements.

sm_advertisements_random (0/1, def 0)
Enable/disable random advertisements. When enabled, advertisements are randomized on every map change and reload.

sm_advertisements_reload
Server command to reload the advertisements.
```

## * Stickers
>You can modify the ConVars below in cfg/sourcemod/csgo_weaponstickers.cfg
### ConVars
```
sm_weaponstickers_flag - Specifies the required flag.
E.g: 'a' for reserved slot.

sm_weaponstickers_overrideview - Specifies whether the plugin will override the weapon view.
P.s: To use your own skins, you must disable this cvar.

sm_weaponstickers_reusetime - Specifies how many seconds it will be necessary to wait to update the stickers again.

sm_weaponstickers_updateviewmodel - Specifies whether the view model will be updated when changing stickers.
P.s: This is necessary so that the player does not need to switch weapons to update the sticker.

```

### Commands
```

```