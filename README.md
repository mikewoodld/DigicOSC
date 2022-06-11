# Digico-OSC
Unofficial and incomplete - logging Digico SD series OSC and other network stuff as I discover it


## iPad App Communication
### DiGiCo Core2 V2 App

   Initial Handshake
   
   1) iPad sends OSC packet from port 57317 to specified IP/Port from app settings (UDP)

          /console/name/?
          
   2) Console Responds 


(more coming here soon)

         
          
### DiGiCo SD App

   Still figuring this one out, it sends a UDP packet with hex 2f 43 6f 6e 73 6f 6c 65 2f 4e 61 6d 65 2f 3f which, when translated, is the same OSC text as the Core2 app. More experimentation will happen

### DiGiCo SD Core2 App (Version 1)

  Same as above. 
  
  
# OSC Packets Sent by Console
(Tested on SD10, these are the OSC packets that are sent when using the "Digico Pad" connection type in External Settings)

## Control Groups

For the following examples, change "1" in the address to be whatever number you need. 

Fader Level

         /Control_Groups/1/fader
         float with current fader level
         
Channel Level Within Control Group

         /Input_Channels/1/CGs_level
         float with level of given channel within a control group
         
Control Group Mute

         /Control_Groups/1/mute
         float with 1 or 0 (mute on or mute off)
         
Control Group Solo

         /Control_Groups/1/solo
         float with 1 or 0 (solo on or solo off)

## Snapshots
         
Current Snapshot Number

         /Snapshots/Current_Snapshot
        int with snapshot number
        
(more soon)

