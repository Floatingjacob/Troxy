# Troxy
Transparent Terraria Proxy

PS5 and Xbox does NOT let you connect to custom Terraria servers. 
This tool is here to fix that problem.
By spoofing itself as a terraria server on your wifi, it allows you to connect to (almost) any terraria server.


HOW TO USE:

using the arduino ide, make sure you have the espressif ESP32 boards installed.
make sure you have the EspMDNS library installed.

the board i tested this code on is the esp32-s2-saola 

after you have all the libraries installed, upload the code to the ESP32.

the ESP32 will boot and host a wifi called 'TerrariaProxyConfig'. connect to it, and open a web browser.
in the web browser, navigate to http://192.168.4.1
you should see a wifi configuration page. enter your wifi credentials, and then hit save.

after your ESP32 connects to your wifi, navigate to http://terrariaproxy.local in a web browser
from there, you should be able to configure where the proxy actually points to and what server it connects you to.

after you have your ESP32 all configured, launch terraria on a console or mobile, and go the the multiplayer tab.
after a few seconds (around 5) you should see a server called 'Terraria', hosted by 'TerrariaProxy'
join it, and you SHOULD be connected to the real terraria server.

## License 📜

This project is under the **GNU General Public License v3.0 (GPL-3.0)**, which means:

- ❌ You **cannot sell** this software without following the rules.  
- 👤 You **must give original credit to me** if you modify it.  
- 🔄 Any derivative work must also use the **GPL-3.0 license**.  

Full license text here: [GPL-3.0 License](https://www.gnu.org/licenses/gpl-3.0.txt)  


CREDITS

Big thanks to Re-Logic for NOT responding to my email asking for help.
The idea for this proxy was originally triggered by my friend Axel, who was complaining that he couldn't connect to custom terraria servers on his PS5.
