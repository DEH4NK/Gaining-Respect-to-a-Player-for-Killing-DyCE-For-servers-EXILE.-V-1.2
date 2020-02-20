////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////                                                                                                                                      //
//                                   Gaining Respect to a Player for Killing DyCE For servers EXILE. V 1.2                              // 
//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
1. Put it along the way:
   addons\DyCE\code\DyCE_respect_killedBots.sqf
   
2. File:
   addons\DyCE\configDyCE.sqf 
   Replace string № 43 
   DyCE_exileRespect = 100; 
   To a new line:
   DyCE_RespectKilledBoat = 100;  
   
3. File:
   addons\DyCE\functions\fn_spawnConvoyAI.sqf
   After line № 151 
   Insert a new line:
   _newUnit addEventHandler ["killed", "[_this select 0, _this select 1] execVM 'Convoy\DyCE\code\DyCE_respect_killedBots.sqf'"];
   
/////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
