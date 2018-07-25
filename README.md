# RPi0W-Server
1. Setup Raspbian Lite
    (i)   Installing/Writing the Raspbian Stretch Lite image file onto the microSD card.
    (ii)  Creating an empty file named "ssh" in the boot partion of the microSD card
    (iii) Creating a wpa_supplicant.conf file in the boot partion as well which contains:
            country=US
            ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
            update_config=1 
            network={
                    scan_ssid=1
                    ssid="xxxxx"
                    psk="xxxxx"
                    proto=WPA
                    key_mgmt=WPA-PSK 
            }
    
2. Setup RTC (DS3231)
3. Setup OLED SS01306
4. Setup LAMP-Webserver
