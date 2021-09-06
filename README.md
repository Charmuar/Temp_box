# Temp_box

-------------------CPE405(T) WEEK1-LAB001-------------------

Hi, everyone 

This project build for education  on Bachelor's degree




         - - - - - - - - - - - - - - 
        | CPE405(T)                 |
         - - - - - - - - - - - - - - 
        | Parkin Thanantthanachon   |
         - - - - - - - - - - - - - - 
        | 61043845                  |
         - - - - - - - - - - - - - - 

        *********************************
        Software : Freecad              *
        Project : Temp box 
        Date    : 6/09/2021



        equipment : 
                        1. NodeMCU ESP8266 V2   X1
                        2. Relay 5 V 1 CH       X1
                        3. Breadboard 170 hole  X1
                        4. connector 5mm. 2     X2
                        5. LED 3 v              X1
                        6. Switch 2 way nc,no   X1
                        7. DHT22                X1


        ----------------------------------------------------------------------------
        | this project have  3 Section fusionm file must build on Freecad Software |
        |                          -------------------------------------------------
        | 1. lid-box    (union)   |
        | 2. mainboard  (union)   |
        | 3. margin-box (union)   |
        --------------------------
                | | 
                \ /
                 v
        list : {
            lid-box : {                                         (Union)
                    lidbox,                                     (Fillet)
                    lid_layer1                                  (Body)
                        }
            mainboard :{                                        (Union)
                    lock-nut-wall-top,                          (Fillet)
                    lock-nut-wall-down                          (Fillet)
                         mainboard_bot :{                       (Union)
                                 margin-breadboard  : {         (Union)
                                         t_l,                   (Union)
                                         t_r,                   (Union)
                                         b_l,                   (Union)
                                         b_r                    (Union)
                                 }
                                 main-nut  : {                  (Union)
                                         bottom_mainboard,      (Body)
                                         breadboard,            (Body)
                                         nut_left_relay,        (Body)
                                         nut_right_relay        (Body)
                                 } 
                        }
                }
             margin-box : {                                     (Fillet)
                    top,                                        (Fillet)
                    bot,                                        (Fillet)
                    right,                                      (Fillet)
                    left,                                       (Fillet)
                    lock-nut-left,                              (Fillet)
                    lock-nut-right                              (Fillet) 
                          }
                                    }
               }
****************************************************************************
        lid-box :{
                width  : 110 mm.
                height : 70  mm.
        },
        lid-layer1 :{
                width  : 110 mm.
                height : 70  mm.
        }, 
****************************************************************************
        lock-wall-top : {
                        width  : 15 mm,
                        height : 25 mm
                        circle(drill) : { 
                                radius :  1.5 mm,
                                height form point : 3.5 mm,
                                width from point : 7.5 mm
                                }
                        }
                }, 
                lock--wall-bot : {
                        width  : 15 mm,
                        height :  25 mm
                        circle(drill) : { 
                                radius :  1.5 mm,
                                height form point : 21.5 mm,
                                width from point : 7.5 mm
                                }
                },
                        mainboard_bot :{
                                    margin-breadboard(all={top,right,left,bot}) : {
                                        width  : 1.5 mm, (4 piece)
                                        height : 7 mm   (4 piece)
                                                main-nut : {
                                                        bottom_mainboard :{
                                                                width  :  110 mm,
                                                                height :  70 mm
                                                        }
                                                        breadboard : {
                                                                width  : 31 mm,
                                                                height : 47 mm
                                                        }
                                                        nut-left-relay :{
                                                                radius : 1.5 mm, (in)
                                                                radius : 2.5 mm (out)
                                                        }
                                                        nut-right-relay :{
                                                                radius : 1.5 mm. (in)
                                                                radius : 2.5 mm (out)
                                                        }
                                                }
                                 }
                        }    
****************************************************************************
        margin-top :{
                width  : 70  mm,
                height : 36  mm
                },
        margin-bot :{
                width  : 70  mm,
                height : 36  mm
                },
        margin-left :{
                width  : 70  mm,
                height : 36  mm
                },
        margin-right :{
                width  : 70  mm,
                height : 36  mm
                }
        left-nut :{
                radius : 1.5 mm,
                height form point : 10 mm,
                width from point  : 10 mm
        }
        right-nut :{
                radius : 1.5 mm,
                height form point : 10 mm,
                width from point  : 10 mm
        }

****************************************************************************




****************************************************************************

        list of references : 

1. NodeMCU ESP8266 V2   
<img src="ref/ESP8266_V2_size/esp8266_v2.png" width="400">


2. Relay 5 V 1 CH      
<img src="ref/RELAY_1_CH_size/relay_1ch_5v.png" width="400">

3. Breadboard 170 hole  
<img src="ref/Breadboard_170hole_size/BreadBoard_170hole.png" width="400">


4. connector 5mm. 2     
<img src="ref/Wire_electric_connector_small_size/wire_connector.png" width="400">


5. LED 3 v            
<img src="ref/LED_5_V_Size/LED_5_V.png" width="400">


6. Switch 2 way nc,no  
<img src="ref/Switch_led_2_way_size/Switch_led_2_way.png" width="400">


7. DHT22            
<img src="ref/DHT22_size/DHT22.png" width="400">


