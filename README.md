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
(Tested on SD10)
