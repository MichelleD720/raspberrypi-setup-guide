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
**note** Will exlain how I fixed the display output to monitor issue

## Prerequisite
- Raspberry Pi board  
- MicroSD card (8GB+ recommended)  
- Micro SD card reader  
- Power supply for the Pi  
- Computer with internet access  
- Wi-Fi network name (SSID) and password  
- Raspberry Pi OS image ([https://www.raspberrypi.com/software/](https://www.raspberrypi.com/software/))
**Optional**
  -HDMI to micro HDMI for monitor
  -monitor
  -keyboard
  -mouse
  -Pi case
**Note** I purchased the 

## Procedure

### 1.Putting the Pi together **Skip to 1.6  if you do not have Pi case
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

1.6 Put your microSD card into the Pi slot and connect the power cable 
![image (5)](https://github.com/user-attachments/assets/a4f5cb7a-459f-48f2-8862-e408afc0ecde)







  
