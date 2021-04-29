# crustySenpais-Left-4-Dead-2-Autoexec
Just my Autoexec so People can use it if they want :)
paste the following in an txt file and rename it to autoexec.cfg (the file extension needs to be .cfg)

     ////////////////////////////////////////////////////////////////////////////////////////////////////////////
    // crustySenpai's autoexec.cfg file									      //
   // put it in here: "C:\Steam\steamapps\common\Left 4 Dead 2\left4dead2\cfg" or wherever you installed it  //
  // also set the config.cfg on "Read Only" if you don't want Settings to be overwritten		    //
 ////////////////////////////////////////////////////////////////////////////////////////////////////////////

                       /////////////////
		      //launchoptions//
                     /////////////////

// go to Steam Libary, rightclick Left 4 Dead 2, click Properties, "Set Launch Options" and paste them there (make a space between each one)

// Removes the Motion Blur when shader effects on high or above
// +mat_motion_blur_percent_of_screen_max 0

// Disables HDR Lighting
// +mat_hdr_level 0

// Skips the Cutscene at startup
// -novid

// Disables Joycons
// -nojoy

// Let the Game use all available Cores
// -useallavailablecores

// Opens the Console directly on startup
// -console

// Change the Game Language
// -language (your language code) - supported languages: en (English), da (Danish), nl (Dutch), fi (Finnish), fr (French), de (German), it (Italian), ja (Japanese), ko (Korean), no (Norwegian), pl (Polish), pt (Portuguese), ru (Russian), zh-CN (Simplified Chinese), zh-TW (Traditional Chinese), es (Spanish), sv (Swedish), hu (Hungarian), tr (Turkish), bg (Bulgarian), cs (Czech), el (Greek), pt-BR (Portuguese - Brazil), ro (Romanian), es-419 (Spanish - Latin American, th (Thai), uk (Ukrainian), vn (Vietnamese)

// Removes the Gore completly (also boost fps)
// -lv

// Disables IPX Support
// -noipx

// Sets the Game on High Priority
// -high

// Not really sure what it does lol
// +precache_all_survivors 1

// Changes the Client Port (should fix issues with "Failed after 10 retrys" Messages)
// +clientport 27619

// Forces the engine to use operating system mouse parameters.
// -noforcemparms

// Forces the engine to use operating system mouse acceleration.
// -noforcemaccel

			 /////////////
			// Settings//
		       /////////////

//For Font Addons (Just change to your resolution)
//mat_setvideomode 1920 1200 1; mat_setvideomode 1440 900 0 //0 = Fullscreen, 1 = Windowed, 2 = Borderless Window

//changes the Brightness of the Game (works only in Fullscreen)
mat_monitorgamma				1.6	// Brightest 1.6 - Darkest 2.6
mat_monitorgamma_tv_enabled			0	// Set to 0 if the game is too bright


//Changes the Viewmodel Fov (change as you want, default 51, personally recommend 70)
cl_viewmodelfovsurvivor				70

//Changes the cl_interp from 0.100 to 0.0167 (100ms - 16.7ms) for better melee deadstops against hunter and jockeys
rate						128000
cl_cmdrate 					128
cl_updaterate 					128
cl_interp 					0.0167
cl_interp_ratio 				1

//General network settings that may helps you when you play in 100 tickrate servers
cl_lagcompensation				1
cl_resend					1.5
cl_timeout					15
net_maxroutable					1200
net_splitpacket_maxrate				50000
net_splitrate					2

//Ping Cap for Server Search (doesn't work i think, maybe just with the old browser?)
//mm_dedicated_search_maxping			100

//Shows net_graph 1 and for Ping, FPS, lerp etc.
net_graph 					1
net_graphproportionalfont 			0
net_graphpos 					1
net_graphheight 				1160

//Makes the Crosshair nice and green
cl_crosshair_alpha 				255
cl_crosshair_blue 				0
cl_crosshair_dynamic 				0
cl_crosshair_green 				255
cl_crosshair_red 				0
cl_crosshair_thickness				2

//Better Thirdperson Aiming
c_thirdpersonshoulderaimdist			360.0
c_thirdpersonshoulderdist			120.0
c_thirdpersonshoulderheight			0.0
c_thirdpersonshoulderoffset			0.0

//Some FPS Tweaks
budget_show_history 				0
cl_detail_avoid_force				0
cl_detail_avoid_recover_speed			0
cl_detail_max_sway				0
cl_perf_wizard_enable				0
cl_ragdoll_limit				0
func_break_max_pieces				0
mat_bloom_scalefactor_scalar			0
mat_grain_scale_override			0
r_PhysPropStaticLighting			0
r_cheapwaterend					1
r_cheapwaterstart				1
r_dynamic					1
r_eyemove					0
r_eyeshift_x					0
r_eyeshift_y					0
r_eyeshift_z					0
r_eyesize					0

//Just general client stuff.
cl_allowdownload				0
cl_allowupload					0
cl_autohelp					0
cl_clearhinthistory				1
cl_downloadfilter				none
cl_forcepreload					1
cl_ideal_spec_mode				4
cl_predictweapons				1
cl_showhelp					0
con_enable					1
gameinstructor_enable				0
joystick					0
sc_enable					0
sc_enable2					0
spec_allowroaming				1

//Some minor changes to the Subtitles to make it appear and disappear faster
cc_lang						english
cc_linger_time					0.5
cc_predisplay_time				0
cc_subtitles					0
closecaption					1
english						1

			 ////////////////////
			// Sound Settings //
		       ////////////////////

snd_musicvolume					0
dsp_enhance_stereo				0
dsp_slow_cpu					0

			 //////////////////
			// Mic Settings //
		       //////////////////

bind "Mouse4" "+voicerecord"
voice_loopback					0		// Set to 1 if you want to hear yourself when you use your mic
voice_enable					1
voice_modenable					1
voice_scale					1
voice_threshold					0
voice_vox					0

			 /////////////
			// aliases //
		       /////////////

//sets you AFK
alias afk "go_away_from_keyboard"

//toggles crosshair
alias crosshair "toggle crosshair 0 1"

//toggle voicechat (doesn't work fully)
alias voice "toggle voice_enable 0 1"

//goes into thirdperson and removes crosshair in it, enables it back in firstperson
alias 3rd "thirdpersonshoulder; toggle crosshair 0 1"

			 //////////////
			// Keybinds //
		       //////////////

//If you want to map your Numpad here are the Keys
// 1 = End 		kp_end
// 2 = Down Arrow 	kp_downarrow
// 3 = Page Down 	kp_pgdn
// 4 = Left Arrow 	kp_leftarrow
// 5 			kp_5
// 6 = Right Arrow 	kp_rightarrow
// 7 = Home 		kp_home
// 8 = Up Arrow 	kp_uparrow
// 9 = Page Up 		kp_pgup
// 0 = Insert 		kp_ins
// . = Delete 		kp_del
// / = (Slash) 		kp_slash
// * = (Multiply) 	kp_multiply
// - = (Minus) 		kp_minus
// + = (Plus) 		kp_plus
// Enter 		kp_enter
// Here you can find all other Keys: https://totalcsgo.com/binds/keys

bind "ALT" "3rd"						//thirdperson
bind "b" "+mouse_menu Warnings"					//Ion's Vocalizer (get it here: https://steamcommunity.com/sharedfiles/filedetails/?id=698857882)
bind "c" "+mouse_menu Reactions"				//
bind "g" "+mouse_menu Misc"					//
bind "h" "+mouse_menu Misc2"					//
bind "i" "+mouse_menu Misc3"					//
bind "j" "+ch1; alias -ch1 -mouse_menu" 			//
bind "k" "+ch3; alias -ch3 -mouse_menu" 			//
bind "l" "+ch5; alias -ch5 -mouse_menu" 			//
bind "m" "+ch2; alias -ch2 -mouse_menu" 			//
bind "n" "+mouse_menu Events"					//
bind "o" "+mouse_menu Misc4"					//
bind "p" "+mouse_menu Misc5"					//
bind "v" "+mouse_menu Enemies"					//
bind "x" "+mouse_menu QA"					//
bind "z" "+mouse_menu Orders"					//
bind "'" "+ch9; alias -ch9 -mouse_menu" 			//
bind "," "+ch4; alias -ch4 -mouse_menu" 			//
bind "." "+ch6; alias -ch6 -mouse_menu" 			//
bind "/" "+ch8; alias -ch8 -mouse_menu"				//
bind "-" "+ch7; alias -ch7 -mouse_menu"				//
bind "=" "+mouse_menu NPC"					//
bind "F4" "afk"							//AFK Hotkey
bind "F5" "disconnect"						//quick disconnect from game
bind "F6" "+mouse_menu Characters"				//Ion's Vocalizer
bind "F7" "show_menu Menu"					//Admin Menu
bind "F8" "voice"						//toggles voicechat
bind "F9" "toggleconsole"					//open the console (on default that key would be "~")
bind "F10" "crosshair"						//toggles the crosshair
bind "F11" "jpeg"						//to make a screenshot duh
bind "F12" "quit"						//closes game

			 /////////////////////
			//  Chat Keybinds  //
                       /////////////////////

//bind "KP_INS" "say thx <3"					//Numpad 0
//bind "KP_DEL" "say I'm Black White guys!"			//Numpad .
//bind "KP_ENTER" "say I have no ammo!"				//Numpad Enter
//bind "KP_PLUS" "say Someone can help me?"			//Numpad +
//bind "KP_MULTIPLY" "say Good luck everyone <3"		//Numpad *
//bind "KP_MINUS" "say GGWP <3"					//Numpad -
//bind "KP_END" "say There's a witch!"				//Numpad 1
//bind "KP_DOWNARROW" "say Smoker!"				//Numpad 2
//bind "KP_PGDN" "say Jockey!"					//Numpad 3
//bind "KP_LEFTARROW" "say Hunter!"				//Numpad 4
//bind "KP_5" "say Splitter!"					//Numpad 5
//bind "KP_RIGHTARROW" "say Charger!"				//Numpad 6
//bind "KP_HOME" "say Tank!"					//Numpad 7

			 /////////////////////
			//  Vote Keybinds  //
                       /////////////////////

//bind "KP_END" "callvote changedifficulty Easy"		//Calls Vote to change Difficulty
//bind "KP_DOWNARROW" "callvote changedifficulty Normal"	//
//bind "KP_PGDN" "callvote changedifficulty Hard"		//
//bind "KP_LEFTARROW" "callvote changedifficulty Impossible"	//
//bind "KP_5" "callvote RestartGame"				//restart the Campain

			 ///////////////
			//  Scripts  //
		       ///////////////

//DSP_Volume Off + Null-Cancelling Script (credits to Xbye: https://steamcommunity.com/sharedfiles/filedetails/?id=487027371)
bind "W" "+mfwd"
bind "A" "+mleft"
bind "S" "+mback"
bind "D" "+mright"

alias +mfwd "dsp_volume 0;-back;+forward;alias checkfwd +forward"
alias +mback "dsp_volume 0;-forward;+back;alias checkback +back"
alias +mleft "dsp_volume 0;-moveright;+moveleft;alias checkleft +moveleft"
alias +mright "dsp_volume 0;-moveleft;+moveright;alias checkright +moveright"
alias -mfwd "-forward;checkback;alias checkfwd none"
alias -mback "-back;checkfwd;alias checkback none"
alias -mleft "-moveleft;checkright;alias checkleft none"
alias -mright "-moveright;checkleft;alias checkright none"
alias checkfwd "none"
alias checkback "none"
alias checkleft "none"
alias checkright "none"
alias none ""

//jump spam (not tested) also from a config from the Site below - mason.cfg
//alias jumppp "+jump;wait;-jump;wait;rejumppp"
//alias +jumpp "alias rejumppp jumppp;jumppp"
//alias -jumpp "alias rejumppp wait"

//bind v +jumpp

			 //////////////////////
			//  Glows Settings  //
		       //////////////////////

//I don't really know who to credit for that because i just found the config on an autoexec archive
//here is the Link: https://sites.google.com/site/left4dead2stuff/customization/autoexec-archive - asfnglows.cfg
//also better just put it into an own cfg so you can simply activate/deactivate it

			 //////////////////////
			//  Survivor Glows  //
		       //////////////////////

//Glow of other survivors
cl_glow_survivor_r 0.0
cl_glow_survivor_g 0.5
cl_glow_survivor_b 1.0

//Glow of hunter when survivor is pounced
cl_glow_ability_r 1.0
cl_glow_ability_g 0.4
cl_glow_ability_b 0.0

//Flashing survivors when capped
cl_glow_survivor_hurt_b 1
alias survivorHurt "incrementvar cl_glow_survivor_hurt_r 0 1 1; incrementvar cl_glow_survivor_hurt_g 0 1 1; wait 15; survivorHurt"
survivorHurt

//Glow of barfed survivors 
//Flashes purple and white, encouraging me to clear them
alias "barfed1" "cl_glow_survivor_vomit_r 1.0;cl_glow_survivor_vomit_g 0.0;cl_glow_survivor_vomit_b 1.0;wait 25;barfed2"
alias "barfed2" "cl_glow_survivor_vomit_r 0.6;cl_glow_survivor_vomit_g 0.6;cl_glow_survivor_vomit_b 0.6;wait 15;barfed1"
barfed1

//Glow of items
alias GlowItem0 "cl_glow_item_r 1; cl_glow_item_g 0; cl_glow_item_b 1"
alias GlowItem1 "cl_glow_item_r 1; cl_glow_item_g 1; cl_glow_item_b 0"
alias GlowItem2 "cl_glow_item_r 0; cl_glow_item_g 1; cl_glow_item_b 1"
alias GlowItemPart0 "GlowItem1; wait 10; GlowItemPart1"
alias GlowItemPart1 "GlowItem2; wait 10; GlowItem0; wait 10; GlowItemRestart"
alias GlowItemRestart "GlowItemPart0"
GlowItemPart0

alias GlowItemFar0 "cl_glow_item_far_r 1; cl_glow_item_far_g 0; cl_glow_item_far_b 1"
alias GlowItemFar1 "cl_glow_item_far_r 1; cl_glow_item_far_g 1; cl_glow_item_far_b 0"
alias GlowItemFar2 "cl_glow_item_far_r 0; cl_glow_item_far_g 1; cl_glow_item_far_b 1"
alias GlowItemFarPart0 "GlowItemFar1; wait 50; GlowItemFarPart1"
alias GlowItemFarPart1 "GlowItemFar2; wait 50; GlowItemFar0; wait 50; GlowItemFarRestart"
alias GlowItemFarRestart "GlowItemFarPart0"
GlowItemFarPart0

			 //////////////////////
			//  Infected Glows  //
		       //////////////////////

//Glow of spawning infected team mates
//Flashes white and dark so it's harder to ignore where team mates are spawning up relative to my position
//alias "ghostinfected" "incrementvar cl_glow_ghost_infected_b 0.0 1.0 1;incrementvar cl_glow_ghost_infected_g 0.0 1.0 1;incrementvar cl_glow_ghost_infected_r 0.0 1.0 1;wait 20;ghostinfected"
//ghostinfected

cl_glow_ghost_infected_r 1.0
cl_glow_ghost_infected_g 1.0
cl_glow_ghost_infected_b 1.0

//Glow of spawned infected team mates
cl_glow_infected_r 0.0
cl_glow_infected_g 0.5
cl_glow_infected_b 1.0

//Glow of barfed on survivors
cl_glow_infected_vomit_r 0.25
cl_glow_infected_vomit_g 0.75
cl_glow_infected_vomit_b 1.00

//Survivor colors
cl_glow_survivor_health_high_r 0; cl_glow_survivor_health_high_g 1; cl_glow_survivor_health_high_b 0
cl_glow_survivor_health_med_r 1; cl_glow_survivor_health_med_g 1; cl_glow_survivor_health_med_b 0
cl_glow_survivor_health_low_r 1; cl_glow_survivor_health_low_g 0; cl_glow_survivor_health_low_b 0
cl_glow_survivor_health_crit_r 1; cl_glow_survivor_health_crit_g 0; cl_glow_survivor_health_crit_b 0.333;

//Health bleed pulse - alternates between temp and perm health
cl_glow_survivor_health_bleed_pulse_amount 0;cl_glow_survivor_health_bleed_pulse 0
alias GlowIncludeBuffer "incrementvar cl_glow_survivor_health_include_buffer 0 1 1; wait 20; GlowIncludeBuffer"
GlowIncludeBuffer


//Glow of items when black and white
alias GlowThirdStrikeItem0 "cl_glow_thirdstrike_item_r 1; cl_glow_thirdstrike_item_g 0; cl_glow_thirdstrike_item_b 1"
alias GlowThirdStrikeItem1 "cl_glow_thirdstrike_item_r 1; cl_glow_thirdstrike_item_g 1; cl_glow_thirdstrike_item_b 0"
alias GlowThirdStrikeItem2 "cl_glow_thirdstrike_item_r 0; cl_glow_thirdstrike_item_g 1; cl_glow_thirdstrike_item_b 1"
alias GlowThirdStrikeItemPart0 "GlowThirdStrikeItem1; wait 10; GlowThirdStrikeItemPart1"
alias GlowThirdStrikeItemPart1 "GlowThirdStrikeItem2; wait 10; GlowThirdStrikeItem0; wait 10; GlowThirdStrikeItemRestart"
alias GlowThirdStrikeItemRestart "GlowThirdStrikeItemPart0"
GlowThirdStrikeItemPart0

			 ////////////
			//  Echo  //
		       ////////////

echo "                                   "
echo "     * * * * * * * * * * * * *     "
echo "    *                         *    "
echo "   *      crustySenpai's       *   "
echo "  *    autoexec.cfg loaded      *  "
echo "   *                           *   "
echo "    *                         *    "
echo "     * * * * * * * * * * * * *     "
echo "                                   "
