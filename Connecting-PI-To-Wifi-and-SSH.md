**Article ID:** KB-RPI-0003  
**Last Updated:** 2025-07-01  
**Author:** Michelle Dang   
**Category:** Raspberry Pi → Remote Access
**Related Articles** 
- [KB-RPI-0001 Hardware-Set-Up](https://github.com/MichelleD720/raspberrypi-setup-guide/blob/main/Hardware-Set-Up.md)
- [KB-RPI-0002 Configuring-Micro-SD](https://github.com/MichelleD720/raspberrypi-setup-guide/blob/main/Configuring-Micro-SD.md)
- [KB-RPI-0004 No-Signal-Display-Monitor](https://github.com/MichelleD720/raspberrypi-setup-guide/edit/main/No-Signal-Display-Monitor)

### 3.Connecting-PI-To-Wifi-and-SSH
3.1 Open up the command line terminal. First one the run box, which is windows key + r. Then type in cmd followed by enter. 
You'll get a black box known as the command prompt

![{54F2D503-7DB1-4175-80BE-BE88ED4F2B66}](https://github.com/user-attachments/assets/93748fa1-a62a-4f7a-8790-8089609add9b)
![{C4CEAA33-1F21-4CFF-BFE6-A063D5893931}](https://github.com/user-attachments/assets/e7f0af45-a8d6-43c3-b776-1dadd5d963aa)

3.2 Now at this point, other tutorials will tell you to try and ping the pi. Their pings will work. Ours will not because the 
raspberrypi5 wants you to use their raspi-config window to set up wifi access.See below,
![{7D94B897-2F2A-4FBD-B722-5A17DD031C78}](https://github.com/user-attachments/assets/24de53be-f735-4e6f-90f7-19bb09fcb180)

3.3 First connect your ethernet cable to you pi and laptop/pc to establish a connection. Now if you try to ping your pi it should do 
a return of something like this. This means that your computer can contact your pi

![{76CA03A6-B236-45B7-8E4A-3CA7FF1AAD79}](https://github.com/user-attachments/assets/0aabdbb5-f008-4e4d-ac98-7c40b7e96d39)


3.3 Now we need to ssh into the pi to configure the wifi setting. 
First type in ssh 'yourusername'@'yourhostname' enter. If you followed along with the tutorial you can copy my screen.
It will ask if you want to create a connection. Type yes.
Now type in the password. It's normal not to see any characters. It's Pi's security feature 
If everything goes well it will output pi@raspberrypi:~ $
![{BDBEDB9E-16C2-4E9E-9C00-3E68143D301A}](https://github.com/user-attachments/assets/a8a4660f-d5f7-43c4-9f36-2af64637033c)

3.4 Now to enter the rasp-config screen. 
Type in sudo raspi-config then hit enter. You should get the blue screen below 
![{34DE0860-D6C5-4553-B3FF-69E74C2C0BCA}](https://github.com/user-attachments/assets/29d5f120-c0f0-4822-a6b0-039dc0c5a56a)

3.5 Use your arrow keys to set up the localization 
Go to 5-> L1-> use the space bar to select your local->use tab to get to the ok button->click enter over the selected local
![{CD065851-5AD8-4E55-87F1-3CA87490224B}](https://github.com/user-attachments/assets/0625d45b-c6d2-4fbf-803d-52b6fab0e238)
![{F8E3F881-85AC-499C-9ED7-C9CB5309964D}](https://github.com/user-attachments/assets/cf56b455-82bb-4e0f-b24f-afb85de5d9cc)
![{09809B49-E97C-4EDB-9DD6-41060D632BA2}](https://github.com/user-attachments/assets/2d061658-9dde-46d0-89e8-53d19e8371dd)
![{2B37BEF2-67E8-4494-A326-F9F4B753034E}](https://github.com/user-attachments/assets/bc4bbf9e-cb30-407d-88a5-a8d16ff55dbc)

3.6 now to set up timezone 
Go to 5-> L2->select your geographic area->select your city/region
![{5AE98035-8D4B-47C6-979A-61AA2E3C9782}](https://github.com/user-attachments/assets/df60e1bf-b67d-4cc0-b6e7-4ca88b8ffcdd)
![{4BD08FA1-F447-4B92-9C16-EFCD0BBC5963}](https://github.com/user-attachments/assets/061831df-1cb3-42b4-aed7-ffff301b9cce)
![{6F663BA0-B75A-4469-807F-EF8EB245EAA5}](https://github.com/user-attachments/assets/17d33b75-aef3-43f9-a9c0-893109a74e0d)

3.7 Now to configure the Legal channels
Go t 5->L4->select your country-> select ok
![{502FAFC1-6E2F-4209-9CBF-32DC19BF81B9}](https://github.com/user-attachments/assets/a8e40ddd-d14c-48d7-b8ee-43da9fcabf1c)


3.8 Now we can set up the wifi
Go to 1->S1->input your wifi name-> input your wifi password
IF you get a message saying Error:Device'' is not a wifi device then go back and redo your 3.5. You probably selected the wrong localization 
Otherwise you should get the message Generation complete
![{1DB4687C-E42E-4AC2-8338-4B277DCF23A7}](https://github.com/user-attachments/assets/01b806f7-95d2-4b71-8257-859d13dd69e9)
![{7C2B0B2D-542F-4CFF-9BE0-D4ADF5FAA426}](https://github.com/user-attachments/assets/acbdc915-8104-49a7-b46b-0af484329842)
![{00CD8CE3-A3EE-44CA-B6A2-5132854DB12E}](https://github.com/user-attachments/assets/b0d27883-2f24-421d-833e-b15e1c070ed6)

3.9 You can unplug your ethernet cable now and try to ping your pi again 
If it looks like the below then congrats your Pi is now connected to wifi. You'll want to write down the IP address for later. 
![{3E1DFDAA-776A-40E0-920B-C38A9A761560}](https://github.com/user-attachments/assets/d49810ed-eb1f-4c1a-8d18-28f90435a273)

3.10 if for some reason it does not appear as an IPv4 address. You can download Advanced IP Scanner and try to find the Pi's IP that way 

















