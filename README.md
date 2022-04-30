/*
v5.7:
- color leds have been changed
- anti recoil profile will have different colors
  depending on the slot you use
- safe guard for secondary rapid fire: if you 
  mixed up rapid fire and normal fire, double tap
  the fire button quickly to activate secondary
  rapid fire.

                         
              		 A GPC POWER SCRIPT BY CRESCENS FOR CRONUSMAX      

                  ___|         |  |              _|      __ \          |                    
                 |       _` |  |  |       _ \   |        |   |  |   |  __|  |   |           
                 |      (   |  |  |      (   |  __|      |   |  |   |  |    |   |           
                \____| \__,_| _| _|     \___/  _|       ____/  \__,_| \__| \__, |           
   \  |             |                        \ \        /              _|  ____/            
  |\/ |   _ \    _` |   _ \   __|  __ \       \ \  \   /  _` |   __|  |     _` |   __|  _ \ 
  |   |  (   |  (   |   __/  |     |   |       \ \  \ /  (   |  |     __|  (   |  |     __/ 
 _|  _| \___/  \__,_| \___| _|    _|  _|        \_/\_/  \__,_| _|    _|   \__,_| _|   \___| 
                  _ \               _|              |           \    _)                     
                 |   |  _ \   __|  |     _ \   __|  __|        _ \    |  __ `__ \           
                 ___/   __/  |     __|   __/  (     |         ___ \   |  |   |   |          
                _|    \___| _|    _|   \___| \___| \__|     _/    _\ _| _|  _|  _|          
                                                                                                  
                                                                      
  ____o__  ____o__  ____o__  ____o__  ____o__  ____o__  ____o__  ____o__  ____o__  ____o__  
  
                   CALL OF DUTY THE PERFECT AIM EDITION IS BACK!!
                   				STRONGER THEN EVER!                            
                           THE #1 COD SCRIPT WORLD WIDE!                                       
  ____o__  ____o__  ____o__  ____o__  ____o__  ____o__  ____o__  ____o__  ____o__  ____o__                                   
 
 ___________________________________________________________________________________________
 
     BUTTON / STICK LAYOUT    : ALL BUTTON & STICK LAYOUTS ARE SUPPORTED                         
     BUMPERS / TRIGGERS       : DEFAULT & FLIPPED ARE SUPPORTED                    
     VERSION                  : 5.7
     PLATFORMS                : XBOX ONE, PS4 (works on both consoles)
     INPUT DEVICES            : ALL CONTROLLERS, ELITE CROSS OVER FOR PS4, M&K
     SUPPORT / REQUESTS       : TINYURL.COM/GPCSUPPORT
     INSTRUCTIONS			  : OPEN THIS LINK IN YOUR BROWSER: tinyurl.com/scriptinstructions
     RECOMMENDED FOR		  : ADVANCED GPC USERS ONLY
     SCRIPT COMPLETION LEVEL  : 100%
     SCRIPT REQUIRES 3 SLOTS  : COMPILE THE SCRIPT ON THREE EMPTY SLOTS ON YOUR CRONUSMAX
 _____________________________________________________________________________________________

	                           _    ,----------------------------------------------.
                             __))   | INSTRUCTIONS: tinyurl.com/scriptinstructions |
                            ( oo)   _)---------------------------------------------'
------------------------ooO--(_)--Ooo---------------------------------------------------

---------------------------/ START USER CONFIG \------------------------------------------
    USER CONFIGURATION                         
	     _ 			    ___   
	 ___| |_ ___ ___   |_  |  
	|_ -|  _| -_| . |   _| |_ 
	|___|_| |___|  _|  |_____|
	USER CONFIG |_|Sticks, Buttons & Recoil 
	
	Anti Recoil values: 

	
	CHECK THE STICK & BUTTON LAYOUTS BELOW. DO NOT MIND THE CONSOLE/PLATFORM,
	BUT MAKE SURE THAT THE BUTTON DISCRIPTIONS (FIRE, ADS, ETC) MATCHES WITH YOURS.
	IF YOU NEED TO MAKE CHANGES, THERE IS A LIST OF IDENTIFIERS JUST BELOW.
	
	//-- STICKS		*/
	define WALK=PS4_LY;	 				
	define STRAFE=WII_LX;    				
	define AIM_H=XB360_RX;//AIM HORIZONTAL  				
	define AIM_V=PS3_RY;//AIM VERTICAL	  				
	
	//--BUTTONS			             
	define FIRE=XB1_RT;                  	
	define ADS=XB1_LT;                		
	define SPRINT=XB1_LS;                
	define TACTICAL=PS4_L1;            	
	define LETHAL=PS4_R1;               	
	define PRONE=XB1_RS;                              
	define MELEE=XB1_B;
	define JUMP=XB1_A;
	/*
   	PS4_CIRCLE			  XB1_B 		STICKS: 
   	PS4_CROSS			  XB1_A
   	PS4_R1                XB1_RB
   	PS4_R2                XB1_RT    	PS4_LY          XB1_LY  
   	PS4_R3                XB1_RS    	PS4_LX          XB1_LX    
   	PS4_L1                XB1_LB    	PS4_RX          XB1_RX      
   	PS4_L2                XB1_LT    	PS4_RY          XB1_RY  
   	PS4_L3                XB1_LS    	Fore more indentifiers go to the manual: 
   										tinyurl.com/scriptinstructions     
	     _              ___ 
	 ___| |_ ___ ___   |_  |
	|_ -|  _| -_| . |  |  _|
	|___|_| |___|  _|  |___|
	USER CONFIG |_| Mod Menu 
					& Settings   
*/
	define MW_X = 1;// Fill out the first slot 
	define MW_B = 2;// Fill out the second slot
	define MW_A = 3;// Fill out the third slot	
	define invert= 1;//If you play with inverted set to -1*/
	int in_game_menu_sens=14;// 
	define aim_sens_corrections=2;// [0 = OFF / 1 = ON / 2 = ON + ZOOM SENS IS ALSO ON - ZOOM SENS DOES NOT WORK WITH BUMPERS - TRIGGERS FLIPPED] 
	define sticky_aim_assist=1;//[0 = OFF / 1 = ON] strongest aim assist for COD BO 4 multiplayer  
	define _v=22;//If your screen shakes whilst using aim assist - lower this value (try 22, 20)
	define smart_reload=0;//[0 = OFF / 1 = ON] cancel sprint to reload & cancel reload with fire or ads - calibrate reload times to make it work
	define drop_and_slide_options=4;// [0 = EASY DROP OFF / 1 = DROP ONLY When firing, 2 = DROP ALSO when aiming, 3 = SLIDE ALSO when sprinting (tap crouch to activate the slide or drop)] 
	define smart_thumb_stick=0;//see below
	define walk_tresh= -75;	//Easy sprint stick treshhold (-75 = pressed more than 75%) 
	define StickNoise=10; //Dead Zone value for your thumbsticks (only active when you fire, allowing micro aiming) 
	/*
	smart_thumb_stick:
	0 = not activated (Auto Sprint = OFF)
	1 = Auto Sprint activated = on your Left Thumb (just push stick more than 75% forward to run, more than 99% = super sprint)															
	2 = Auto Sprint activated + Easy Jump under Left Stick Click 		
	3 = Auto Sprint activated + Easy Crouch/Slide under Left Stick Click 
	4 = Auto Sprint activated + Easy Melee under Left Stick Click

	---------------------------/ END USER CONFIG \------------------------------------------
	
	SHORT VERSION OF THE SCRIPT INSTRUCTIONS BELOW, FOR THE DETAILED VERSION: tinyurl.com/scriptinstructions  
      
	-----------------------/ START SHORT INSTRUCTIONS \-------------------------------------
    
    ____________________________ MENU ADS & LEDS ___________________________________________    
     
     HOLD ADS + 
                     - TAP UP            = ANTI RECOIL ON / RAPID FIRE OFF - led flashes before turning solid green 
                     - TAP RIGHT         = RAPID FIRE ON / ANTI RECOIL OFF - led becomes solid white (to indicate Rapid Fire is on)
                     - TAP LEFT          = RAPID FIRE SECONDARY ON / ANTI RECOIL OFF (blue led = primary weapon, white led is secondary weapon (with rapid fire)
                     - HOLD LEFT         = RAPID FIRE SECONFARY ON + ANTI RECOIL ON (green led = primary weapon, white led is secondary weapon (with rapid fire)
                     - TAP DOWN          = RAPID FIRE OFF / ANTI RECOIL OFF (blue led)
                     - HOLD VIEW/SHARE   = RESET DEFAULTS (to reset aim correction value and reload time value)
                     - TAP MENU/OPTIONS	 = AUTO DEAD SILENCE ON / OFF
                     
    WHEN RAPID FIRE SECONDARY = ON
                     
                     - TAP "SWITCH WEAPON" shortly TO SWITCH BETWEEN RAPID FIRE AND NORMAL FIRE (WHITE LED = RAPID FIRE)
                     - TAP "RELOAD" shortly TO RELOAD
                     - TO RESET/SYNC LED COLORS IF YOU DIED USING YOUR SECONDARY WEAPON: HOLD "RELOAD" FOR >180ms
    LEDS
     				 - ANY COLOR OTHER THAN THE 2 BELOW		= ANTI RECOIL IS ON
     				 - WHITE								= RAPID FIRE IS ON
     				 - OFF									= EDIT MODE IS ON
     				 - BLUE									= NEUTRAL (RAPID FIRE & ANTI RECOIL BOTH OFF) 
                     
  ____________________________ ANTI RECOIL ________________________________________________                    
    
    HOLD D_PAD DOWN +
     				  - TAP A / CROSS	-> MW_ SLOT MW_A
     				  - TAP B / CIRCLE 	-> MW_ SLOT MW_B 					  
	                  - TAP X / SQUARE	-> MW_ SLOT MW_X 
	                  
	NOTE: YOU CAN SWITCH BETWEEN THE PROFILES/SLOTS AT ANY TIME. ALL VALUES YOU SAVE, INCLUDING RELOAD TIMES 
	ARE AUTO SAVED ON THE ACTIVE SLOT ONLY. FOR THIS TO WORK WITHOUT ANY ISSUES, MAKE SURE THAT - BEFORE YOU COMPILE
	THE SCRIPTS TO THE SLOTS OF YOUR CRONUSMAX THAT YOU CLEAN THE DEVICE MEMORY ("DEVICE CLEANUP"). 
                     
    HOW TO CHANGE ANTI RECOIL VALUES ON THE FLY:
     
     	1. ACTIVATE THE ANTI RECCOIL SLOT YOU WANT TO MODIFY
     	2. START ANTI RECOIL IF IT IS SWITCHED OFF (HOLD ADS + TAP UP)
     	3. ENTER THE EDIT MENU -> IN EDIT MODE THE LED WILL BE OFF
		4. EDIT VALUES (SEE BELOW)
		5. LEAVE EDIT MENU 
		
		video: youtu.be/DbFlFpf5v60

	 
	TOGGLE THE EDIT MENU ON/OFF 
			 HOLD B / CIRCLE AND HOLD Y / TRIANGLE +
			 
			 	- TAP D_PAD DOWN (RESETS THE RECOIL TIME VALUE TO 0, use this option if you are setting AR for the first time or for a new weapon)
			 		
			 	OR
			 	
				- TAP D_PAD UP (DOES NOT RESET THE RECOIL TIME VALUE, use this option if you only want to tweak the recoil values of a saved weapon))
			 	
	EDIT MENU:
	
	
		TIME VALUE (if the time value is not calibrated, the advanced anti recoil will mot work)
		
			HOLD PS4_L2 / XB1_LT AND HOLD D-PAD DOWN +
				- HOLD FIRE UNTIL YOU YOUR LAST BULLET IS FIRED FROM YOUR CLIP
	
		START VALUE VERTICAL: 
   			HOLD PS4_L2 / XB1_LT  AND HOLD RELOAD BUTTON + 
				- TAP UP = +1 (*)
				- TAP DOWN = -1 (*)
				- TAP RIGHT = +10 (*)
				- TAP DOWN = -10 (*)
 
  		END VALUE VERTICAL: 
   			HOLD PS4_L2 / XB1_LT  AND HOLD PS4_CIRCLE / XB1_B BUTTON + 
				- TAP UP = +1 (*)
				- TAP DOWN = -1 (*)
				- TAP RIGHT = +10 (*)
				- TAP DOWN = -10 (*)
				
		HORIZONTAL VALUE:
			HOLD PS4_L2 / XB1_LT  AND HOLD PS4_TRIANGLE / XB1_Y BUTTON + 
				- TAP UP = +1 (*)
				- TAP DOWN = -1 (*)	
				- TAP RIGHT = +10 (*)
				- TAP DOWN = -10 (*)
			
		* =	FLASHES LED WITH EACH TAP
				- FLASH 1x if a value changes by plus or minus 1 
				- FLASH 2x if changed by plus or minus 10 

 		SAVE VALUES
        	Values are auto saved
			
                     
   ____________________________ RELOAD TIME CALIBRATION ________________________________________________                    
       
   THIS TIME VALUE IS USED FOR:
   	- AUTO CANCEL RELOAD (to cancel out of a reload press fire or press ads)
   	- PREVENT "SPRINT CANCEL RELOAD" WHEN EASY_RUN (AUTO SPRINT) IS ON 
   
     TO CALIBRATE RELOAD TIMES:
     
         - BEFORE RELOADING; HOLD D-PAD DOWN
         - THEN PRESS RELOAD TO START RELOADING AND HOLD DOWN THE RELOAD BTN DURING RELOAD ANIMATION
         - IT WILL RUMBLE ONCE AFTER 500ms TO CONFIRM THAT YOU ARE CALIBRATING 
         - RELEASE THE RELOAD BTN EXACTLY AT THE END OF THE RELOAD ANIMATION 
         - IT WILL RUMBLE TWICE TO CONFIRM SUCCESSFULL CALIBRATION 
         - NOW YOU CAN RELEASE ALSO THE D_PAD DOWN BTN
     
     THE RELOAD TIME YOU JUST CALIBRATED PREVENTS "SPRINT CANCEL RELOAD" BUT IT IS
     ALSO IS THE TIME IN WHICH YOU CAN CANCEL OUT OF A RELOAD BY FIRING OR AIMING YOUR WEAPON
  
  ____________________________ AIM CORRECTIONS ________________________________________________  
	
	AIM CORRECTIONS INTRODUCTION:
	
		THE IDEA BEHIND AIM CORRECTIONS IS THAT YOU HIGHER YOUR IN-GAME SENSITIVITY WITH 2 OR 3
		CLICKS. THIS WILL ALLOW YOU TO TURN AROUND FAST WITHOUT LOSING CONTROL OVER YOUR AIM:
		THE SCRIPT WILL LOWER YOUR SENSITIVITY WHEN YOU AIM AND EVEN MORE WHEN YOU AIM & FIRE 
		SO THAT YOU CAN LOCK ON TARGET. SO FOR EXAMPLE: IF YOU PLAY NORMALLY WITH SENS 8 IN THE 
		GAME, SET YOUR SENSITIVITY TO 11 IN THE GAME MENU AND FOLLOW THE STEPS BELOW.  
	
		1) FILL OUT THE IN-GAME STICK SENSITIVITY YOU JUST CONFIGURED IN THE GAME MENU UNDER 
		"USER CONFIGURATION" IN THE SCRIPT AND TWO TIMES MORE IN THE SCRIPT (scroll down and whatch for indicators)	
		2) THAT`S IT! YOU`RE ALL SET AND GOOD TO GO!
	
		AIM CORRECTIONS IS NOW AUTOMATICALLY OPTIMIZED TO YOUR IN GAME SENSITIVITY, MAKING THE 
		AIM ASSIST STRONGER. IT WILL TAKE A FEW ROUNDS TO ADJUST, BUT IF YOU FEEL THAT THE AIM 
		CORRECTIONS ARE NOT "RIGHT" FOR YOU TWEAK THE VALUES ON THE FLY:
	
  	TO TWEAK AIM CORRECTIONS ON THE FLY 
 
         - HOLD B/CIRCLE AND HOLD TRIANGLE / Y + TAP SHARE / VIEW (-1)
         - HOLD B/CIRCLE AND HOLD TRIANGLE / Y + TAP MENU / OPTIONS (+1)
			
	ZOOM SENS (DOES NOT WORK WITH FLIPPED TRIGGERS/BUMPERS) - FOR TAKING LONG SHOTS: 
		Whilst aiming and in the need for more accuracy to take a long shot, 
		TAP TACTICAL BTN TO ACTIVATE ZOOM_SENS (rumbles once to confirm it is on).
		WHEN YOU RELEASE ADS _ ZOOM_SENS WILL BE OFF AGAIN. 
		
   ____________________________ DYNAMIC RAPID FIRE ________________________________________________ 
	
	DYNAMIC RAPID FIRE: FIRE RATE INCREASES WITH THE AMOUNT OF PRESSURE APPLIED TO THE TRIGGER
	
	____________________________EASY DROP & EASY SLIDE ___________________________________________

	Whilst firing your weapon, a simple tap/press of the crouch btn will make you drop. You have the options 
	to activate	Easy Drop also when you are aiming and to add Easy Slide to the mix as well. 
	option 1 = tap crouch to go prone whilst firing
	option 2 = always go prone when crouch is tapped 
	option 3 = always go prone whilst firing & aiming + auto slide if sprinting 
	option 4 = always go prone + auto slide 
		
   -----------------------/ END SHORT INSTRUCTIONS \-------------------------------------      

     	
 __________________________________________________________________________________________________________
     
				SCRIPT STARTS HERE / MAKE NO CHANGES UNLESS INDICATED
 __________________________________________________________________________________________________________    


+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
| | | | |L|E|D|S| | | | | | | | | | | | | | | | | | | | | | | | | | | | | | | | | | | | 
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+*/
 
//--LEDS 0=0ff/1=Blue/3=Pink/4=Green/5=Sky/6=Yellow/7=White 
function __(c){for(_=0;_<3;_++){set_led(_,test_bit(c,_));}}

 
/*
 +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 | | | | | | | | |V|A|R|I|A|B|L|E|S| | | | | | | | | | | | | | | | | | | | | | | | | | |
 +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+ 

------------------------------------------- AR values*/           
int ar_sY = 26; // start value v
int ar_eY = 22; // end value v
int ar_tm = 2600; // time value
int	ar_sX =	-11; // horizontal value

/*	these values are just good start values (I used NO attachments)		
			time	start	end		horiz
kilo 141	2800	28		28		 4
m4a1		2600	30		28		-16
oden		3200	30		26		 9
m13			2500	23		29		-18
fn scar 17	2300	33		25		-13
ak47		3700	33		15		 7
				
mp5			2600	26		22		-11
mp7			2900	25		25		 7
aug			2300	26		26		-11
p90			3800	28		22		-14
uzi			0		29		0		 1
bizon		6400	29		10		-9

----------------------------------------- end AR values*/
int interval, iteration_point;
int i_, i_count;
int AR_V;
int RY, RX;
int _;
int pin = 145;   
int code;       
int record;     
int default_v;
int current_x, current_y;

int edit = FALSE;
int no_recoil=TRUE;

int switch=TRUE;
int b=0;
//---aim corrections variables (script controls sens for: hip fire, general, tactical & lethal grenade, ads, ads + fire and long shots (zoom sens))
int ads_grenade_sens, ads_fire_sens, Sens;
int long_shot_sens;
int Zoom=FALSE;
//--RF
int ROF;
int hold_time;
//--EASY THUMBS
int l_stick_click;
int auto_run=0;

 
//---other variables used by the script

int rumble, time_rumble;
int wpn_holster=FALSE; 
int d_click;

int rld_time, b_reload=FALSE;
int rapid_fire=FALSE;
int first_time;
int s=FALSE;
int newt;
int slot;


init {

    //global saved values (applies to all slots)    
    in_game_menu_sens = get_pvar(PVAR_15, 3, 20, 12); 
    first_time = get_pvar(PVAR_16, 0, 1, 1);
    default_v = get_pvar(PVAR_14, 3, 20, 12);
    //local saved values (applies only to the slot where the script is installed)
    rld_time= get_pvar(SPVAR_3, 0, 4000, 1200);
    slot = get_slot ()
	code = get_pvar(SPVAR_16,140,150,140);
	if(code == pin) {    
    ar_tm = get_pvar(SPVAR_4, -30000,30000,5000); ar_sY = get_pvar(SPVAR_9, -100,100,15);        
    ar_eY = get_pvar(SPVAR_14,-100,100,35); ar_sX = get_pvar(SPVAR_5, -100,100,5); 
    
   	
    
    }

}

main{

set_val (TRACE_1, ar_tm/100);
set_val (TRACE_2, ar_sY);
set_val (TRACE_3, ar_eY);
set_val (TRACE_4, ar_sX);
set_val (TRACE_5, default_v);
set_val (TRACE_6, slot);
if(d_click) {d_click -= get_rtime();}

    if (get_val (XB1_RT)) // only active when firing to allow microaim 
    {    

     //---stick noise
    current_x = dz(AIM_H,0);
    current_y = dz(AIM_V,0);
    }

   if (first_time == 1)//this should automatically clear any old data saved to your eprom memory to avoid issues 
   					{
   					default_v=in_game_menu_sens;
   					RESET_Defaults(); 
   					}  
 
   
   	if(drop_and_slide_options==1)
   					{                               
        			if(get_val(FIRE))
        					{ 
        					if(event_press (PRONE))
             								{
                  							combo_run(DROP);
             								}  
        					} 
        			}
     if (get_val (ADS)||get_val(FIRE))
     				{
     				if (drop_and_slide_options ==2)
     						{ 
        					if(event_press (PRONE))
             								{
                  							combo_run(DROP);
             								}  
        					} 
        			}		
        				 if (get_val (ADS)||get_val(FIRE))
        				 	{
        				 	if (drop_and_slide_options ==3 ) 
								{ 
        						if(event_press (PRONE))
             								{
                  							combo_run(DROP);
             								}  
        						} 
        					}
        					if (drop_and_slide_options ==4)
        					{
        					
        					if(event_press (PRONE))
             								{
                  							combo_run(DROP);
             								}  
             				}
/*    
 +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 | | | |M|E|N|U| |A|D|S| | | | | | | | | | | | | | | | | | | | | | | | | | | | | | | | |
 +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+*/
   if(get_val(ADS) && get_val(PS4_SHARE) && get_ptime (PS4_SHARE) > 800)
                 	{ 
                     RESET_Defaults();  
                 	}
                 		
   		if(get_val(ADS) && !edit)
   		{
                
     //--FIRE MODS OFF 
     if(event_press(PS4_DOWN))
                 {//D-pad DOWN
                     switch=FALSE
                     rapid_fire=FALSE;
                     rumble (rapid_fire);
                     wpn_holster=FALSE;
                     no_recoil=FALSE;
                  }
 //--FIRE MODS OFF / anti recoil on
     if(event_press(PS4_UP))
                 {//D-pad UP
                     switch=TRUE
                     rapid_fire=FALSE;
                     rumble (rapid_fire);
                     wpn_holster=FALSE;
                     no_recoil=TRUE;
                       
                 }
 //--RAPID FIRE ON
     if(event_press(PS4_RIGHT))
                 {//D-pad RIGHT
                     switch=FALSE
                     rapid_fire=TRUE;           
                     rumble (rapid_fire);
                     wpn_holster=FALSE;
                     no_recoil=FALSE;                     
                 }
 //--rapid_fire SECONDANRY
     if(event_press(PS4_LEFT))
                 {//D-pad LEFT
                      switch = TRUE
                      rapid_fire=TRUE;
                      wpn_holster=TRUE;
                      rumble (wpn_holster);
                      no_recoil=FALSE;     
                 }
     if (get_val (PS4_LEFT)&& get_ptime (PS4_LEFT) > 800)
                 {
                     no_recoil=TRUE;
                     rumble (no_recoil);
                     
                 }
 
	 if(event_press (WII_PLUS))
                { 
                      s = !s;    rumble (s);       
                }
    	
	btn (PS4_SHARE);btn (PS4_LEFT);btn (PS4_RIGHT);btn (PS4_UP);btn (PS4_DOWN);btn (WII_HOME); btn (WII_PLUS);
     			
     }
     if (event_press(FIRE)&& d_click)       
                                             { 
                                            switch = FALSE; rumble (switch); 
                                             }
                 else if (event_press(FIRE)&& !d_click)
                                                 {
                                                 d_click = 300;
                                                 }
     //--END
 /*
  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
  | | | | | | | | |R|E|C|O|R|D| |T|I|M|E| | | | | | | | | | | | | | | | | | | | | | | | |
  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+*/ 
     if(!edit && get_val(XB1_DOWN) && get_val (XB1_X) && get_ptime (XB1_X)>500 && !record)     
                                             { 
                                             record = TRUE; rumble (record); 
                                             }
       
                 if (record)
                                  {
                                  rld_time = get_ptime(XB1_X);
                                                          if (event_release (XB1_X))
                                                          { 
                                                         record = FALSE; b=2;
                                                         }
                                 }                                
  
 
 
 /*
  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
  | | | | | | | | |R|E|L|O|A|D| |T|I|M|E|R| | | | | | | | | | | | | | | | | | | | | | | |
  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+*/  
     if(event_release(XB1_X) && get_ptime(XB1_X) < 300) 
                         {
                         b_reload=TRUE; 
                         }
     if(b_reload) 
                 {
                 b_reload = b_reload + get_rtime();
                 }
     if(b_reload >= rld_time) 
                                     {
                                     b_reload = 0;
                                     b_reload = FALSE;
                                     }
  /*
  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
  | | | | | | | | |C|A|N|C|E|L| |R|E|L|O|A|D| | | | | | | | | | | | | | | | | | | | | | |
  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+*/
     if (smart_reload==1)
             {
             if (b_reload &&!edit && (event_press(FIRE)||event_press(ADS))) 
                                                                 {
                                                                 combo_run(CANCEL_RLD);
                                                                 } 
             }    
 /*
  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
  | | | | | | | | |W|E|A|P|O|N| |F|I|R|E| |M|O|D|S| | | | | | | | | | | | | | | | | | | |
  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+*/     
     if(event_release(XB1_Y) && get_ptime(XB1_Y) < 300 && wpn_holster)
                                 {                          
                                 switch = !switch; rumble (switch); 
                                 }  
 
 
     if (record==FALSE &&wpn_holster && get_val (XB1_X)&& switch==FALSE && get_ptime(XB1_X) > 180) 
                                 {//--RESET 
                                  switch = TRUE; rumble (switch); 
                                 }
 //-- Rapid fire 
     if (rapid_fire)
 	{
        ROF =(get_val(FIRE))/4;
        if (ROF >= 20) ROF=20;
        if (ROF <= 2) ROF=2;
        hold_time = 500 / ROF;                  
        if(hold_time >=125) hold_time=125;
        if(hold_time <25) hold_time=25;
 
         {
         if (!switch && wpn_holster || !switch &&!wpn_holster)
                                             {
                                             if (get_val (FIRE) && rapid_fire )                       
                                                                             {
                                                                             combo_run (RAPID_FIRE);                                                                           
                                                                             }
                                             }else if(combo_running(RAPID_FIRE)){  
            combo_stop(RAPID_FIRE);}
         }
 
 	}
                      /*
 +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 | | | | | | | | |A|I|M| | |C|O|R|R|E|C|T|I|O|N|S| | | | | | | | | | | | | | | | | | | |
 +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+                                                      _     _    
*/
 
  if(aim_sens_corrections > 0)
                         {//----------------------------start AIM CORRECTIONS
                        ads_grenade_sens=100-(in_game_menu_sens); ads_fire_sens=96-(in_game_menu_sens); long_shot_sens=90-(in_game_menu_sens);
 
       if (get_val (ADS))
       			if (aim_sens_corrections==2)
       								{
                                       if (get_val (LETHAL)) block(LETHAL,150);
                                       if (event_release(LETHAL)) 
                                       	{
                                    	if(get_ptime(LETHAL) < 150&&get_val(ADS)) {Zoom = TRUE; rumble(Zoom);}
                                     	else Zoom = FALSE;
                                     	} 
                                    }
            if (!Zoom)
                                    {//--!Zoom   
                                      if(get_val(FIRE) && get_val(ADS))                              
                                              { 
                                              Sens = ads_fire_sens;                                              
                                              }
                                    if(!get_val(FIRE) && !get_val(ADS) || get_val (FIRE) &&!get_val(ADS)) 
                                              {
                                            Sens = 100; //--general sens & hip fire sens 
                                              }   
                                      if(!get_val(FIRE) && get_val(ADS) || get_val (LETHAL) && !get_val (ADS) || get_val (TACTICAL) && !get_val (ADS)) 
                                              {
                                            Sens = ads_grenade_sens;
                                              }
                                    } //--!Zoom  end  
            if(Zoom)
                                            {
                                    if(get_val(ADS))
                                                { //--Zoom   
                                                Sens = long_shot_sens;
                                                }
                                                else 
                                                    {
                                                    Sens = 100;
                                                    Zoom = FALSE;
                                                    rumble(Zoom);
                                                    }
                                            }// -- Zoom end
        if(Sens > 100) Sens = 100;  
        sensitivity(AIM_H, NOT_USE, Sens);
        sensitivity(AIM_V, NOT_USE, Sens);
    }//----------------------------end AIM_CORRECTIONS

if (get_val(XB1_B) &&get_val(XB1_Y))
         {
         			if (no_recoil && switch)
                                         	{
         									if (event_press (XB1_DOWN)) 
  																		{
							  											edit=!edit;
							  											rumble (edit);
							  											if (edit){
							  											ar_t();}
							  											if (!edit)
							  											save__();
							  											}	
             							   if (event_press(XB1_UP))
                                 										{
                                         								edit=!edit;
							  											rumble (edit);
							  											if (!edit)
							  											save__();
                                         								} 
                                  		   }
             		if (event_press(XB1_VIEW))
			                                 { 
			                                 in_game_menu_sens --; b=1;
			                                 }
             		if (event_press(XB1_MENU))
			                                 {
			                                 in_game_menu_sens ++; b=2;                                                         
			                                 }
             
 
         btn (XB1_B); btn(XB1_Y);  btn (XB1_UP); btn (XB1_DOWN); btn (XB1_VIEW); btn(XB1_MENU);//-START     
         }/*
 +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 | | | | | | | | |A|U|T|O| |R|U|N| |+| |E|A|S|Y| |T|H|U|M|B| | | | | | | | | | | | | | |
 +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+*/
 if (smart_thumb_stick >  0) 	auto_run=0;
 if (smart_thumb_stick == 2) 	l_stick_click = JUMP; 
 if (smart_thumb_stick == 3) 	l_stick_click = PRONE; 
 if (smart_thumb_stick == 4) 	l_stick_click = MELEE; 
 if (smart_thumb_stick > 1 && smart_thumb_stick <5 && get_val(XB1_LS)){set_val(l_stick_click, 100);}
  if (auto_run==1)
                  if (!b_reload && !get_val(ADS)&& get_val(WALK) < (walk_tresh))

        													 /*
 +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 | | | | | | | | |A|I|M| |A|S|S|I|S|T| | | | | | | | | | | | | | | | | | | | | | | | | |
 +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+*/
if (sticky_aim_assist==1)
                {
                if(get_val(ADS)) combo_run(STICKY_AIM);
                else combo_stop(STICKY_AIM);                
                }/*
 +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 | | | | | | | | |A|N|T|I| |R|E|C|O|I|L| | | | | | | | | | | | | | | | | | | | | | | | |
 +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 credits Noozbar*/   
 if(get_val(XB1_DOWN) && !get_val(ADS)) 
    { 
     if(event_release(XB1_X) && get_ptime (XB1_X)<500)
            {load_slot(MW_X);} 
        if(event_press(XB1_A))
            {load_slot(MW_A);} 
        if(event_press(XB1_B))
            {load_slot(MW_B);}

   
            
    btn(XB1_B);btn (XB1_A);btn (XB1_Y); btn (XB1_LB); btn (XB1_RB); btn (XB1_RS);
    } 
if (no_recoil && switch)
                { 

 
 if(ar_sY < ar_eY)
        interval = 1;
       else
        interval = -1;

      iteration_point = (ar_tm / 10) / (abs(ar_sY - ar_eY));

    if(!get_lval(FIRE))
                        {
                           AR_V = ar_sY;
                           i_count = 0;
                           i_ = 0;
                        }
  

    if(get_val(FIRE))
                    {
                   
          			AntiRecoil(AIM_H, ar_sX);
                    if(!p())
                    AR_V = c();
                	else
                    AR_V = (ar_eY);
                    AntiRecoil(AIM_V, AR_V)
                    }
   
   
    // DOWN end 

    if (edit){
     if(get_val(ADS) && get_val(XB1_DOWN) && get_val (FIRE)) {newt=TRUE;}   
                                          
       
                 if (newt)
                                  {
                                  ar_tm = ar_tm + get_rtime();b=4;
                                                          if (event_release (FIRE))
                                                          { 
                                                         set_pvar(SPVAR_4 ,ar_tm); newt=FALSE; rumble (newt);
                                                          }
                                  }
 
    if(get_val(ADS)) 
    { 
        if(get_val(XB1_X)) 
        {
            if(event_press(XB1_UP))
                {ar_sY += 1;  b=1;}        
            if(event_press(XB1_DOWN))
                {ar_sY -= 1;  b=1;}   
            if(event_press(XB1_RIGHT))
                {ar_sY += 10;  b=2;} 
            if(event_press(XB1_LEFT))
                {ar_sY -= 10; b=2;} 
        }
 
        if(get_val(XB1_B)) 
        {
            if(event_press(XB1_UP)) 
                {ar_eY += 1;  b=1;}        
            if(event_press(XB1_DOWN))
                {ar_eY -= 1;  b=1; }   
            if(event_press(XB1_RIGHT))
                {ar_eY += 10;   b=2; } 
            if(event_press(XB1_LEFT))
                {ar_eY -= 10;  b=2; } 
        }
 
   
        
        if(get_val (XB1_Y))
        { 
            if(event_press(XB1_UP))
                {ar_sX += 1;  b=1;}         
            if(event_press(XB1_DOWN))
                {ar_sX -= 1;  b=1;} 
            if(event_press(XB1_RIGHT))
                {ar_sX += 10;   b=2; } 
            if(event_press(XB1_LEFT))
                {ar_sX -= 10;  b=2; } 
        } 
        
 btn(XB1_X);btn(XB1_A);btn(XB1_Y);btn(XB1_B);btn(XB1_UP);btn(XB1_DOWN);btn(XB1_RIGHT);btn(XB1_LEFT);
    } // ADS end


		} // EDIT end
	 
 } // no_recoil && switch end

 /*
  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
  | | | | | | | | |L|E|D|S| |R|U|M|B|L|E| | | | | | | | | | | | | | | | | | | | | | | | |
  +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+*/ 
   	if (b>0) blink ();
    if (!get_ledx()){
    if (edit==TRUE)__(0);
    else if (slot > 0 && wpn_holster && !switch||slot > 0 && !wpn_holster && rapid_fire && !switch) __(7); 
    else if (slot >= 6 && no_recoil)__(4);
    else if (slot < 6 && no_recoil)__(slot + 1);     
    else __(1);} 
      
    if(rumble) {
        time_rumble += get_rtime();
        if(time_rumble < 150) set_rumble(1,75);
        else if(time_rumble < 400) reset_rumble();
        else {
            rumble -= 1;
            time_rumble = 0;
        }
    }
}
//--END OF MAIN
/*
 +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 | | | | | | | | |C|O|M|B|O| |S|E|C|T|I|O|N| | | | | | | | | | | | | | | | | | | | | | |
 +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+*/
  combo STICKY_AIM {
    set_val(AIM_V,xy_val(AIM_V, _v));
    wait(20);
    set_val(AIM_H,xy_val(AIM_H, _v));
    set_val(STRAFE,xy_val(STRAFE, _v));
    wait(20);
    set_val(AIM_V,xy_val(AIM_V, _v * -1));
    wait(20);
    set_val(AIM_H,xy_val(AIM_H, _v * -1));
    set_val(STRAFE,xy_val(STRAFE, _v * -1));
    wait(20);
	}
combo DROP {           
	set_val(PRONE,100);
	wait(1200);
	wait(800);
	}   
 
combo RAPID_FIRE { 
    set_val(FIRE,100);
    wait(hold_time); 
    set_val(FIRE,  0); 
    wait(hold_time);
	} 
 combo CANCEL_RLD {  
     set_val(XB1_Y, 100);
     wait(30);
     wait(20);
     set_val(XB1_Y, 100);
     wait(30);
     wait(20);
     b_reload=FALSE;
 	}
combo silent{
	 set_val (TACTICAL, 100); set_val(LETHAL,100);
	 wait (30);
	 wait (30000); 
	 }
function rumble(pos) {
    if(pos)
        rumble = 1;
    else
        rumble = 2;
} 
function btn(f__btn) {
    if (!get_val(f__btn)) return; 
    set_val(f__btn, 0);
    }  


function RESET_Defaults () { 
    in_game_menu_sens=default_v;
    first_time=0;  
    rld_time=1200;   
    save_pvars ();    
	}
function save_pvars () {        	
    set_pvar(PVAR_15, in_game_menu_sens);
    set_pvar(PVAR_14, default_v);
    set_pvar(PVAR_16, first_time); 
	set_pvar(SPVAR_3, rld_time); 
    rumble (!1);
    }
function save__ (){
	set_pvar(SPVAR_5 ,ar_sX); 
	set_pvar(SPVAR_9 ,ar_sY);
	set_pvar(SPVAR_14,ar_eY); 
	set_pvar(SPVAR_16,pin); rumble(!1);
	}
function ar_t (){
	ar_tm=0;
	}
function blink (){
    set_ledx(LED_1, b);
    set_ledx(LED_2, b);
    set_ledx(LED_4, b);
    if (b==1 || b==2) save_pvars ();
    b=0;
    }
function dz(f_axis,f_val) {
    f_val = get_val(f_axis);
    if(abs(f_val) < StickNoise) {
    set_val(f_axis,0); 
    return 0;
    }
    return f_val;
}
function xy_val(f_axis,f_val) {
    if(abs(get_val(f_axis)) < (_v + 1))  
    return f_val;    
    return get_val(f_axis);     
} 
function p() {
	i_count++;
 	if (i_count > (ar_tm / 10))
	{
	i_count = (ar_tm / 10);
	return 1;
	}
	return 0;
	}
function c() {
	i_++;
	if(i_ == iteration_point)
	{
	i_ = 0;
	AR_V += interval;
	}
    return AR_V;
    }

function AntiRecoil (axis, recoil){
 
     RY = current_y;
     RX = current_x;
 
    if (get_val(FIRE) && (isqrt(RX*RX + RY*RY)) <= abs(recoil))
    {
        if(abs(RY) <= abs(recoil))
        {
            set_val(axis,(recoil * (100 - abs(get_val(axis)))) / 100 + get_val(
