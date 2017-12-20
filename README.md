Jakelli's CS:GO Config
This is my constantly updated CS:GO autoexec config. Changelogs can be found under revisions here

Put autoexec.cfg in ...\Steam\steamapps\common\Counter-Strike Global Offensive\csgo\cfg or take what you want from it and add to your autoexec config.

Launch Options
-novid -freq 144 -refresh 144 -tickrate 128 -maxplayers_override 50 -nojoy -nod3d9ex1 +exec autoexec.cfg
Enter launch options at Steam > Library > Counter-Strike: Global Offensive (right-click) > Properties > Set Launch Options...

Other Settings
Windows Sensitivity: 6/11
Mouse DPI: 900
Mouse Polling Rate: 1000hz
1280x960 4:3 stretch
In-Game Audio Ouput: Headphones

Weapon Loadout
CT: M4A4, USP-S, CZ75-AUTO
T: CZ75-AUTO

Questions?
I can't recieve notifications for gists so your question or comment may go unanswered for a while. Instead you can reach out to me on Twitter (@jakellli)

Raw
 autoexec.cfg
// jakelli's CS:GO config
// Updated 12/20/17

// Rates
rate "307200"
cl_cmdrate "128"
cl_updaterate "128"
cl_interp "0.0"
cl_interp_ratio "1"
cl_interpolate "1"
cl_lagcompensation "1"

// Mouse
sensitivity "1.14"
zoom_sensitivity_ratio_mouse "1.0"
m_rawinput "1"
m_customaccel "0"
m_mouseaccel1 "0"
m_mouseaccel2 "0"
m_mousespeed "0"

// Crosshair
cl_crosshair_drawoutline "0"
cl_crosshair_dynamic_maxdist_splitratio "0.35"
cl_crosshair_dynamic_splitalpha_innermod "1"
cl_crosshair_dynamic_splitalpha_outermod "0.5"
cl_crosshair_dynamic_splitdist "7"
cl_crosshair_outlinethickness "1"
cl_crosshair_sniper_show_normal_inaccuracy "0"
cl_crosshair_sniper_width "1"
cl_crosshair_t "0"
cl_crosshairalpha "255"
cl_crosshaircolor "5"
cl_crosshaircolor_b "0"
cl_crosshaircolor_g "0"
cl_crosshaircolor_r "255"
cl_crosshairdot "0"
cl_crosshairgap "-2.000000"
cl_crosshairgap_useweaponvalue "0"
cl_crosshairscale "0"
cl_crosshairsize "2"
cl_crosshairstyle "4"
cl_crosshairthickness "1"
cl_crosshairusealpha "1"
cl_fixedcrosshairgap "-4.5"

// View Model
cl_viewmodel_shift_left_amt "1.5"
cl_viewmodel_shift_right_amt "0.75"
viewmodel_fov "68"
viewmodel_offset_x "2"
viewmodel_offset_y "2"
viewmodel_offset_z "-1.300000"
viewmodel_presetpos "0"
cl_bob_lower_amt "21"
cl_bobamt_lat "0.33"
cl_bobamt_vert "0.14"
cl_bobcycle "0.98"

// Video
mat_queue_mode "-1" // auto detect multi-core rendering
fps_max "999"

// Audio
voice_enable "1"
voice_scale "0.18"
lobby_voice_chat_enabled "0" // voice chat in lobby

// Buy Binds
bind "kp_enter" "buy ak47; buy m4a1;"
bind "kp_plus" "buy vesthelm;"
bind "kp_minus" "buy awp;"
bind "kp_multiply" "buy smokegrenade;"
bind "kp_pgup" "buy hegrenade;"
bind "kp_rightarrow" "buy flashbang;"
bind "kp_pgdn" "buy molotov; buy incgrenade;"
bind "kp_del" "buy decoy;"
bind "kp_slash" "buy vest;"
bind "kp_uparrow" "buy p250;"
bind "kp_5" "buy tec9; buy fiveseven;"
bind "kp_downarrow" "buy deagle;"
bind "kp_ins" "buy defuser;"
bind "kp_end" "buy galilar; buy famas;"
bind "kp_leftarrow" "buy ssg08;"
bind "kp_home" "buy mp7;"

host_writeconfig // write settings to config.cfg
echo ""
echo ""
echo "autoexec.cfg executed"
echo ""
echo ""
echo ""
// Buy binds in separate cfg
exec buybinds.cfg

Raw
 practicecfg.cfg
// Move the this file to C:\Steam\steamapps\common\Counter-Strike Global Offensive\csgo\cfg
// When you have started a local game server, open the console and type: exec practicecfg

// Server config
sv_cheats 1
mp_limitteams 0
mp_autoteambalance 0
mp_roundtime 60
mp_roundtime_defuse 60
mp_maxmoney 60000
mp_startmoney 60000
mp_freezetime 0
mp_buytime 9999
mp_buy_anywhere 1
sv_infinite_ammo 1
ammo_grenade_limit_total 5
bot_kick
mp_warmup_end

//Practice
sv_grenade_trajectory 1
sv_grenade_trajectory_time 10
sv_showimpacts 1
sv_showimpacts_time 10

// binds
bind “N” “noclip”
bind “M” “give weapon_hegrenade;give weapon_flashbang;give weapon_smokegrenade;give weapon_incgrenade;give weapon_molotov;give weapon_decoy”
bind “O” “cast_ray”

mp_restartgame 1

echo “”
echo “”
echo “”
echo “########## JAKELLI'S PRACTICE CONFIG LOADED ##########”
echo “”
echo “”
echo “”
