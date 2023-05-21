# ESP_remote_PC_switch

ESP8266 based Cloud Remote Switch which uses Arduino Cloud IoT as PaaS provider. This switch acts as a remote power and reset switch for PC or any other electronic device which is located far away from the operator's location.

![Things Dashboard](https://github.com/skillsheen/ESP_remote_PC_switch/assets/133706254/df93ff24-21bb-4287-87a7-5a671c6e16fe)

This ESP8266 based Remote Power switch contains the following:
    Disk State
    Power State
    Power Switch
    Reset Switch
    
![Cloud Dashboard](https://github.com/skillsheen/ESP_remote_PC_switch/assets/133706254/46cf0842-c529-4e12-bdef-ff377f214dde)
    
The "Switch" is boolean Read and Write command which sends True or False command from the Arduino Cloud IoT to the ESP board inturn translating to High or Low signal. This results in power/reset switch to act as a pressed switch.

The "State" is boolean Read command which receives High or Low signal from the ESP board to the Arduino Cloud IoT inturn translating to True or False command . This results in power state and disk state to display the status in the Arduino Cloud IoT dashboard.

The "PC State time" which is a Cloudcounter shows the PC Power State in timeline. It logs the total time the PC is in ON state. This informs user the exact time when  the PC Power was turned OFF or got Shut down abruptly.

