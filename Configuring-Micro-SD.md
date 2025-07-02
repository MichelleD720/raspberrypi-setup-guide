**Article ID:** KB-RPI-0002  
**Last Updated:** 2025-06-30  
**Author:** Michelle Dang   
**Category:** Raspberry Pi → Configurations

**Related Articles** 
- [KB-RPI-0001 Hardware-Set-Up](https://github.com/MichelleD720/raspberrypi-setup-guide/blob/main/Hardware-Set-Up.md)
- [KB-RPI-0003 Connecting-PI-To-Wifi-and-SSH](https://github.com/MichelleD720/raspberrypi-setup-guide/blob/main/Connecting-PI-To-Wifi-and-SSH.md)
- [KB-RPI-0004 No-Signal-Display-Monitor](https://github.com/MichelleD720/raspberrypi-setup-guide/blob/main/No-Signal-Display-Monitor.md)
- [KB-RPI-0005 New_PWD_And_Hostname](https://github.com/MichelleD720/raspberrypi-setup-guide/edit/main/New_PWD_And_Hostname.md)

### 2.Configuring the microSD card
2.1 Insert your microSD card into your reader and connect to your laptop or PC.

2.2 Go to https://www.raspberrypi.com/software/ and download for windows 
![{E68B2ABF-DA8B-460A-B440-E48C915D71FB}](https://github.com/user-attachments/assets/3e3a1cc5-178a-440f-b8fc-19f542cf3d33)

2.2 Now open the RaspberyPi imager. You'll want to select the RaspberryPi 5 then the 64 bit OS and 
your MicroSD card. If there is no microSD card option shown then unplug and replug your reader. This will more than likely fix the issue. If that doesn't work, the issue could be hardware related, so try a different card or reader if you have one.
![{251C0540-A884-4F9A-B166-782A52DEDA5A}](https://github.com/user-attachments/assets/3841c1d0-b799-4b9d-a5d9-3376567a7a79)

2.3 Go to edit setting we will now set up the card, so have a place to write down information ready. You'll also need to know your WIFI SSID (wifi name) and password. 
![{B62F8D32-5BED-4DD0-B542-28A3E64899B6}](https://github.com/user-attachments/assets/f051b527-9729-4233-a528-556c4835f0b5) 

2.4 For now copy what I have for the hostname. The password will be raspberrypi. All of these can be changed later once you've completed inital set up and remote access. 
Input your own information for the username, SSID, password, Wireless LAN country, timezone, and keyboard layout 
### WARNING:use a username you want because it is a pain to change later, unless you want to create a new user and disable the inital setup one
![{35CA1F3F-C2D8-4CBC-91EC-53A5F7939B03}](https://github.com/user-attachments/assets/1a90bb59-05fb-4d77-87fa-f4fe026571c4)

2.5 Go to services and enable SSH and click save and wait for it to finish
![{1960863F-7DDB-43ED-A7BF-6F98A51450B1}](https://github.com/user-attachments/assets/3864b5c9-fcfd-4b44-b570-fd8dbcd84f94)

2.6 Go to the usb drive icon and eject the SD card. Now you can safely remove it from your reader.  
![{FEA66462-8A5C-4BB1-A705-F04400BB7ACA}](https://github.com/user-attachments/assets/936eade0-b7a2-461a-ae21-4e0551322e56)
![{F6CD433A-07EB-4EC2-9D4C-1E60BCF533C2}](https://github.com/user-attachments/assets/4c4d1f08-8a34-4a43-8590-b4fbf64b3ec7)

2.7 Put your microSD card into the Pi slot and connect the power cable 
![image (5)](https://github.com/user-attachments/assets/a4f5cb7a-459f-48f2-8862-e408afc0ecde)
