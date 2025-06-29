# raspberrypi-setup-guide
Headless Raspberry Pi setup guide for Wi-Fi configuration and remote access

**Article ID:** KB-RPI-0001  
**Last Updated:** 2025-06-28  
**Author:** Michelle Dang   
**Category:** Raspberry Pi → Initial Setup  

## Purpose
This article outlines how to set up a Raspberry Pi using a headless method (no monitor), connect it to Wi-Fi, and access it from a desktop computer via SSH. It also documents real obstacles I faced during the setup process—such as networking issues and SD card troubleshooting—to help others avoid the same pitfalls.

## Obstacles 
- Couldn’t find the fan’s connection port. **Skip to 1.1**
- Ports misaligned, making it hard to fit the Pi into the case. **Skip to 1.4**  
- No display output, so switched to headless setup.  
- Trouble connecting to Wi-Fi and locating IP/MAC addresses.  
- Initial SSH connection failures required troubleshooting.
#### Note 
I will explain how I fixed the display output to monitor issue and also I am a windows user. 

## Prerequisite
- Raspberry Pi board  
- MicroSD card (8GB+ recommended)  
- Micro SD card reader  
- Power supply for the Pi  
- Computer with internet access
- Ethernet cable
- Wi-Fi network name (SSID) and password  
- Raspberry Pi OS image ([https://www.raspberrypi.com/software/](https://www.raspberrypi.com/software/))
### Optional
  -HDMI to micro HDMI for monitor
  -Monitor
  -Keyboard
  -Mouse
  -Pi case
#### Note 
I purchased the Vilros "WAVE" Raspberry Pi 5 Compatible Aluminum Alloy Active + Passive Cooling Case, it's just okay. 

## Procedure

### 1.Putting the Pi together **Skip to 2.7 if you do not have Pi case
1.1 If you have the optional Pi case, take the cover lid off of the fan power supply pins 
![image](https://github.com/user-attachments/assets/e2a7c8c0-aefd-4107-a07a-f49af144a980)

1.2 Attach the thermal pad to the contact point shown below 
![image (1)](https://github.com/user-attachments/assets/73fe7a19-0487-48e4-855a-2bb943a105be)

1.3 Connect the fan to it's power supply; Don't brute force it, direction does matter!
![image (2)](https://github.com/user-attachments/assets/f4182a31-4fae-4946-b3e2-1bd354e9490a)

1.4 Slide the Pi into the case port side in first and lightly press down until it is in
**Note** The pi may not look like it's in all the way or may look misalgined that it fine
![image (3)](https://github.com/user-attachments/assets/6209ecd0-1743-4239-9bc1-488517d0071d)
![image (4)](https://github.com/user-attachments/assets/81bf80fc-f1a8-4422-93c7-f9a7a3c0a1c6)

1.5 Put the case cover on and screw it in. If you want too include the Micro SD card cover you can, but I reccommend doing that after you finish all the inital set up steps. Once screwed in the components should settle into  place and now have a fully assembled Pi

### 2.Configuring the microSD card
2.1 Insert your microSD card into your reader and connect to your laptop or PC.

2.2 Go to https://www.raspberrypi.com/software/ and download for windows 
![{E68B2ABF-DA8B-460A-B440-E48C915D71FB}](https://github.com/user-attachments/assets/3e3a1cc5-178a-440f-b8fc-19f542cf3d33)

2.2 Now open the RaspberyPi imager. You'll want to select the RaspberryPi 5 then the 64 bit OS and 
your MicroSD card. If there is no microSD card option shown then unplug and replug your reader. This will more than likely fix the issue. If that doesn't work, the issue could be hardware related, so try a different card or reader if you have one.
![{251C0540-A884-4F9A-B166-782A52DEDA5A}](https://github.com/user-attachments/assets/3841c1d0-b799-4b9d-a5d9-3376567a7a79)

2.3 Go to edit setting we will now set up the card, so have a place to write down information ready. You'll also need to know your WIFI SSID (wifi name) and password. 
![{B62F8D32-5BED-4DD0-B542-28A3E64899B6}](https://github.com/user-attachments/assets/f051b527-9729-4233-a528-556c4835f0b5) 

2.4 For now copy what I have for the hostname and username. The password will be raspberrypi. All of these can be changed later once you've completed inital set up and remote access. 
Input your own information for the SSID, password, Wireless LAN country, timezone, and keyboard layout 
![{35CA1F3F-C2D8-4CBC-91EC-53A5F7939B03}](https://github.com/user-attachments/assets/1a90bb59-05fb-4d77-87fa-f4fe026571c4)

2.5 Go to services and enable SSH and click save and wait for it to finish
![{1960863F-7DDB-43ED-A7BF-6F98A51450B1}](https://github.com/user-attachments/assets/3864b5c9-fcfd-4b44-b570-fd8dbcd84f94)

2.6 Go to the usb drive icon and eject the SD card. Now you can safely remove it from your reader.  
![{FEA66462-8A5C-4BB1-A705-F04400BB7ACA}](https://github.com/user-attachments/assets/936eade0-b7a2-461a-ae21-4e0551322e56)
![{F6CD433A-07EB-4EC2-9D4C-1E60BCF533C2}](https://github.com/user-attachments/assets/4c4d1f08-8a34-4a43-8590-b4fbf64b3ec7)

2.7 Put your microSD card into the Pi slot and connect the power cable 
![image (5)](https://github.com/user-attachments/assets/a4f5cb7a-459f-48f2-8862-e408afc0ecde)

## Connecting PI to wifi and SSH 












  
