# Phantom manual synchronization with infrared LEDs

## Contents
- synchronization of two camera phantoms: settings, electric circuit, and parameters
- Operating system: Windows 10 
- Software used: PCC 3.4
- Phantoms cameras: Phantom Miro M11O, Phantom VEO E310

## How it works: 
1. Triggering of VEO camera by fly falling in the field of the camera 
2. Triggering of the two infrared LEDs
3. Triggering of Miro camera by the led in the camera field 
4. Manual synchronization afterwards with the lighting of the LEDs (one led in each field of view/ two cameras). 

## Step 1: Connect your computer to the phantoms
- You will need two ethernet ports for the two cameras or one ethernet port + a USB/ethernet adapter
- Connect the two cameras to the ethernet ports. 
- Go to Settings > Network & internet ([screenshot](https://user-images.githubusercontent.com/100707728/156572474-bb176024-39ee-4cec-b7cc-db82da4b3e4e.png))
- Find bellow "Advanced network settings" > Network and Sharing center  ([screenshot](https://user-images.githubusercontent.com/100707728/156572632-586b0638-dcf2-47ad-b19e-c21ecf24a661.png))
- In the panel to the left find "Change adapter settings" ([screenshot](https://user-images.githubusercontent.com/100707728/156573019-e449b3e7-94cd-4932-b5fb-e103908bccc9.png))
- This is where you will change the ethernet settings of both cameras to connect them to your computer. You will need the IP address of both cameras.
- Double click on the ethernet connection you want to modify (if you don't know which camera corresponds to which ethernet port plug and connect the cameras one by one). This will open the windows: "Ethernet properties".
- Find "Protocole Internet version 4 (TCP/IPv4)" and double click. Click on "Use the following IP address:" and complete the three lines with the IP address of your camera. It should look something like this [screenshot](https://user-images.githubusercontent.com/100707728/156538293-bd518ba3-276e-48d5-8bc5-71dbf7e93030.png). Click "Ok"
- Do the same thing for the other camera. 

## Step 2: Install and open PCC
- Website of PCC: https://www.phantomcamera.fr/resourcesandsupport/phantomresources/pccsoftware

## Step 3: Infrared electric circuit 
- Trigger detection on the VEO camera, P5 port, with P5 in " recording " mode: see in this [image](https://user-images.githubusercontent.com/100707728/156549922-d30fde64-473d-4005-b435-d5d9c6516db7.png). 

- Infrared LED circuit: see this very basic [diagram](https://user-images.githubusercontent.com/100707728/156557324-e85e71c7-09cf-4f59-9858-1ebf81a579b8.png). When the VEO camera is triggered the signal light the two infrared LEDs and the Miro camera is triggered. 

## Step 4: PCC parameters 
See the [screenshot](https://user-images.githubusercontent.com/100707728/156555562-c006bb96-4320-4dcf-a2eb-31f31e56c202.png): how I trigger the two cameras. Note that my camera where oriented at 90°. The VEO camera was triggered by the fly falling in the field of the camera while the miro camera was triggered when the Infrared LED lights up. 

> 1. Miro:
- Miro camera setting in PCC to change the signal of the port P5: see [image](https://user-images.githubusercontent.com/100707728/156550670-4fa0779d-3cff-4d8a-a129-bc22f25b675b.png)
- Settings: see this [screenshot](https://user-images.githubusercontent.com/100707728/156557653-f084d75e-e565-48ba-bffc-63030c6c2bdb.png)

> 2. VEO:
- Settings: see this [screenshot](https://user-images.githubusercontent.com/100707728/156557793-a7deb19f-9708-4fdd-9f60-70fee769d141.png)

## Step 5: save in multipage tiff
