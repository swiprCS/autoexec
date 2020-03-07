// start

cl_color 3
rate 786432
cl_cmdrate 128
cl_updaterate 128
cl_interp 0
cl_interp_ratio 1

fps_max 999

net_graph 1
net_graphproportional font 0

// mutes enemy
cl_mute_enemy_team 1

// adds buys overhead
+cl_show_team_equipment

// forces always show inventory
cl_showloadout 1

// disables motd ads
cl_disablehtmlmotd 1

// smoke xhair
bind mouse4 "toggle cl_crosshairsize 1000 3"

bind "o" "say ¯\_(ツ)_/¯"
bind "p" "say (╯°□°）╯︵ ┻━┻)"
bind "[" "say ns. (҂◡_◡)"
bind "]" "say stab stab <==[]=C(ړײ)‎​​"
bind "l" "say ( ° ͜ʖ͡°)Ɑ͞  ̶͞ ̶͞ ̶͞ ̶͞ ̶͞ ̶͞ ̶͞ ̶͞ ̶͞ ̶͞ ̶͞ ̶͞ ̶̶͞͞ ̶ ﻝﮞ"

bind m "buy p250;drop"
// bind , "buy ump45;drop"
bind , "buy mp9; buy mac10;drop"

bind F4 "buy hegrenade; buy smokegrenade; buy molotov; buy incgrenade; buy flashbang;"

bind mwheelup +jump
bind mwheeldown +jump

// grenade binds
bind "z" "use weapon_hegrenade;"
bind "x" "use weapon_flashbang;"
bind "c" "use weapon_smokegrenade;"
bind "v" "use weapon_molotov;use weapon_incgrenade;"

bind tab "+showscores;r_cleardecals"

// jumpthrow
alias "+jumpthrow" "+jump;-attack"
alias "-jumpthrow" "-jump"
bind "alt" "+jumpthrow" 

// crouch jump
alias +cjump "+jump; +duck"     
alias -cjump "-jump; -duck"
bind space +cjump

// volume toggle
bind home "toggle volume .01 .8"

// crosshair
cl_crosshaircolor "1"

// cross crosshair
cl_crosshairdot "0"
cl_crosshairgap "-2"
cl_crosshairgap_useweaponvalue "0"
cl_crosshairscale "0"
cl_crosshairsize "3"
cl_crosshairstyle "4"
//cl_crosshairthickness "1"
cl_crosshairthickness 1.3
cl_crosshairusealpha "1"
cl_crosshair_drawoutline "1"
//cl_crosshair_drawoutline "0"

// custom stuff
//viewmodel_offset_x "2.5"
//viewmodel_offset_y "-3"
//viewmodel_offset_z "-2"
//viewmodel_fov "68"
//viewmodel_presetpos "4"

// removes the shifting of the arm when crouching down.
//cl_viewmodel_shift_left_amt "0"
//cl_viewmodel_shift_right_amt "0"

// removes the bobbing of the weapon back and forth, when you run.
//cl_bob_lower_amt "0"
//cl_bobamt_lat "0"
//cl_bobamt_vert "0"

// huntsman
//cl_viewmodel_shift_left_amt "0.500000"
//cl_viewmodel_shift_right_amt "0.250000"
//viewmodel_fov "54"
//viewmodel_offset_x "2.5"
//viewmodel_offset_y "-2"
//viewmodel_offset_z "-2"

// karambit
cl_viewmodel_shift_left_amt "0.500000"
cl_viewmodel_shift_right_amt "0.250000"
viewmodel_fov "54"
viewmodel_offset_x "2.400000"
viewmodel_offset_y "-1.500000"
viewmodel_offset_z "-0.700000"

viewmodel_presetpos "0"
viewmodel_recoil "1.0"
cl_bob_lower_amt "5.000000"
cl_bobamt_lat "0.100000"
cl_bobamt_vert "0.100000"
cl_bobcycle "0.98"
cl_crosshair_sniper_width 2

// to keep stickers looking right
cl_righthand 1 

// to toggle to left hand.. Keep stickers looking correct
bindtoggle end cl_righthand

// seangares radar
cl_hud_radar_scale "1.15";
hud_scaling "0.850000";
hud_showtargetid "1";
cl_radar_always_centered "1";
cl_radar_icon_scale_min "0.6";
cl_radar_scale "0.42";
cl_radar_square_with_scoreboard "1";
cl_radar_always_centered "0";
cl_radar_icon_scale_min "0.6";
cl_radar_rotate "1";

// dmg given
developer "0"
con_filter_text "Damage Given"
con_filter_text_out "Player:"
con_filter_enable "2"

// Mouse
m_rawinput "1"
m_mouseaccel1 "0"
m_mouseaccel2 "0"
m_mousespeed "0"
sensitivity "2.1"
zoom_sensitivity_ratio_mouse "1.0"

cl_buywheel_nomousecentering 1

// doesn't allow E to open buy menu
cl_use_opens_buy_menu "0"

bind rwin "say_team I pressed the Windows key! Tabbing back into the game."
bind lwin "say_team I pressed the Windows key! Tabbing back into the game."

clear

// end
host_writeconfig
