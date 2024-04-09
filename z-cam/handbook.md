---

title: Z Handbook
menu_order: 1
post_status: publish
post_excerpt: This is a post excerpt
featured_image: _images/post-image.jpg
taxonomy:
    category:
        - resources/z-cam/
        - resources
    post_tag:
        - Z CAM


---

# Handbook 

## Z Cam Community Handbook


This handbook was made using my own experiences with my E2 and E2 F8, as well as the collective knowledge of the members of the Z Cam E2 Facebook group, it’s by no means complete but it is a good starting point if you are new to Z Cam. The quick FAQ below addresses most of the questions I see new members ask when joining the Facebook group, after that is a more detailed guide on each of the cameras, features, and software. Keep in mind I do not own every model of camera, so if you see an innacuracy in your model, please try to correct it for others to see.




## Z CAM Official Resources
**Resources on Z Cam's Github**
- [Basic Info](https://github.com/imaginevision/Z-Camera-Doc/blob/master/E2/intro.md "")
- [How to Sync E2 Cinema Camera (M/I/S Explained)](https://github.com/imaginevision/Z-Camera-Doc/blob/master/E2/howto/E2%20Sync%20Cable%20-%20Quick%20User%20Guide.pdf)
- [How to sync Timecode on Z Cam E2 Cinema Camera](https://github.com/imaginevision/Z-Camera-Doc/blob/master/E2/howto/Z-CAM-E2-Synchronize-time-code-with-external-device.pdf)
- Communication Protocols
  - [HTTP on E2 and Flagships](https://github.com/imaginevision/Z-Camera-Doc/blob/master/E2/protocol/http.md)
  - [HTTP on Z Cam E1](https://github.com/imaginevision/Z-Camera-Doc/blob/master/E1/http.md)
  - [LANC on E2 - Uses Sony's LANC Protocol](https://github.com/imaginevision/Z-Camera-Doc/blob/master/E2/protocol/lanc.md)
  - UART - [Commands](https://github.com/imaginevision/Z-Camera-Doc/blob/master/E2/protocol/uart/uart_command.md) - [db9 pin info ](https://github.com/imaginevision/Z-Camera-Doc/blob/master/E2/protocol/uart/db9_pin.md) - [Camera UART Pinout (Tx,Rx,5V, Ground)](https://github.com/imaginevision/Z-Camera-Doc/blob/master/E2/protocol/uart/ctrl_pin.jpg)
- 3D Models of Z Cams - [E2c](https://github.com/imaginevision/Z-Camera-Doc/raw/master/E2/design/E2C_3D.zip) - [E2](https://github.com/imaginevision/Z-Camera-Doc/raw/master/E2/design/E2_3D.zip) - [E2 M4](https://github.com/imaginevision/Z-Camera-Doc/raw/master/E2/design/E2-M4_3D.zip) - [E2 S6](https://github.com/imaginevision/Z-Camera-Doc/raw/master/E2/design/E2-S6_3D.zip)


**Resources on Z Cam's Website**
- [E2C User Manual (up to Firmware 0.93)](https://drive.google.com/file/d/1ABLlbGBeXCJOu-rnCrjw1tevuDleDyoM/view "E2C")
- [E2 User Manual (up to firmware 0.89)](http://www.z-cam.com/wp-content/uploads/2019/10/Z-CAM-E2-User-Manual-draft-v0.6-FW0.89-.pdf "E2")
- [Flagship (M4, S6, F6, F8) User Manual (up to firmware 0.93)](http://www.z-cam.com/wp-content/uploads/2020/04/Z-CAM-E2-Flagship-Series-User-Manual-draft-v0.2-FW0.93-.pdf "Flagship")
- [How to color calibrate a Z Cam - also fixes stuck/dead pixels](http://www.z-cam.com/wp-content/uploads/2020/07/Z-CAM-E2-Hot-Pixel-Calibration-v1.2_draft.pdf "How")


## FAQ



### How to Upgrade Firmware On Z CAMs
Note it is NOT possible to rollback to a firmware before 0.95 once you have updated to 0.95 or newer. My handbook only includes 0.94 and newer, since I strongly encourage all users to be on the most up to date firmware for best performance.
> My preferred way to connect my Z Cam to my computer is with a USB C cable and connecting to the web browser, since it requires no installs and gives you the same basic features as the desktop application.


1. Connect to 172.18.18.1/www/index.html in your browser.
   > Be sure your USB mode is set to Network in the Connection Menu in camera.
   
2. On the webpage you can control the camera or playback. Select Controller.
   > The latest firmware for each camera is found in the Firmware Downloads section above.
   
3. Navigate to the Misc Menu, click Upgrade and then select the file you downloaded from Z Cam’s website in the prompt.
   > If upgrading from a firmware previous to 0.95 then you MUST rename the .fw file extension to .zip The reason for this is that .fw did not exist prior to 0.95 and it is changed going forward to mitigate Mac and Safari from automatically unzipping downloaded .zip files.
   





### What is Z Cam Native ISO  
>The Z Cam E2 and flagships have dual native ISO, while the E2C and E2G only have one native ISO. Here is a chart listing them. If you want to film exclusively in these ISOs, change ISO Control in the Exposure Menu to Native ISO.


| Camera  | Low Native ISO  |  High Native ISO |
| :------------ | :------------: | :------------: |
| F8 & S6  | 400  | 1250  |
| F6  | 400  | 2500  |
| E2 & M4 WDR Off<br>E2 & M4 WDR on  | 500<br>250  | 2500<br>1250  |
|  E2G & S6G | 1250  | -  |
| E2c  |  800 | -  |


### How to Expose for Zlog
  - 1st read [Jason's Medium Post](https://medium.com/@jasonzhang_22759/the-design-of-log-curve-20541efda7fe) on the LOG design curve.
   

  - Next, familiarize yourself with the False Color Spectrum of Z CAMs
  > As a general rule you want to make sure your image is free from orange, purple, and blue while in false color mode. The neon green is where you want to aim to get your middle grey exposure, as this leaves 7 stops above to deal with over exposure. All skin tone exposure values in the scene should fall between the neon green and yellow regions.




### Sample Kits



Z Cam Flagship Sample Kits
#### Z Cam E2 F8 Sample Kit


This build focuses on taking advantage of the 8k resolution of the camera. It would be best used for stock footage or for a heavily cropped editing style. This is similar to my setup for client work where I film in 8k and deliver in 4k, because the F8 allows me to crop 4x without any loss in quality.


    Camera – Z Cam E2 F8
    Cage – User preference, mine is Nitze Flagship cage
    Recording Media – Angelbird if CFAST, Sandisk if external SSD
    Battery – Powerextra 6600mAh battery with DC and USB outputs
    Monitor – Swit 7 inch 3000nit – super bright 7 inch monitor so you can clearly see every pixel in frame no matter your environment
    Lenses – Zeiss Milvus or Otus primes for tack sharp 8k images. If you shoot in 8k and deliver in 4k then I would recommend getting the Canon EF 16-35 F/4 lens with image stabilization. With the potential of a 4x edit crop it turns this 16-35 lens into a 16-140mm while still being true 4k and having a stabilized image. If you are spending the money to get the F8 over the F6 put money into glass that takes advantage of this choice.
    Handles
        Right side – Portkeys Keygrip – use with this cable to power and control the follow focus.
        Left side – user preference, a wooden rosette mount handle works well, or an inverted handle from a shoulder mount for a more compact rig.
    Follow Focus – Nucleus M motor only – Milvus lenses have such a long focus throw that the nucleus nano struggles to push it unless over-volted, so it’s best to just get the M.
    Audio – Deity D3 or D3 Pro if input to camera and want audio dial control. If you want an external audio recorder I would opt for the Zoom H6, which you would feed the line out into audio input of the Z Cam for a scratch track and sync the audio from the recorder in post.
    Tripod – Cayer fluid head tripod with carbon fiber legs – With my F8 rig on this I can still pickup the tripod one handed to reposition the setup.


#### Z Cam E2 F6 Sample Kit



This build focuses on being a one person production unit with the ability to go from shoulder rig to tripod with ease. What the F6 lacks in resolution compared to the F8 it makes up for in frame rates


- Camera - **Z Cam E2 F6**


  **Camera** – Z Cam E2 F6


  **Cage** – User preference, mine is Nitze Flagship cage


  Recording Media – Angelbird if CFAST, Sandisk if external SSD
  Battery – Powerextra 6600mAh battery with DC and USB outputs for the camera and NP-F570 batteries to power your side focus handle.
  Monitor – Atomos Ninja V if you want camera control & external recording, Portkeys BM5 if you only need camera control. Swit 7 inch 3000nit if you want a bigger and brighter monitor and don’t need touchscreen camera control.
  Lenses – User preference of full frame coverage lenses depending on the look you’re going for, some of my favorites are a vintage set of prime cine-mod soviet era glass from Ironglass, Tokina Cinema Vista 16-28mm for a wide zoom option, and the Tamron SP 24-70mm F/2.8 is also a great choice if you need more focal lengths covered by a zoom lens and also have lens stabilization.
    Handles
        Right side – Portkeys Keygrip – use with this cable to power and control the nucleus m.
        Left side – Tilta Side Focus handle with rosette mount for over-volting and control of the nucleus nano. Skip this if you only need 2 focus controls and prefer a manual follow focus.
    Follow Focus – Both Nucleus M motor only and Nucleus Nano motor only – you’ll be using the M on which ever of the focus, zoom or aperture gears that need the most torque, and the nano on the other. If you have a need for a third follow focus on your rig I would get this manual one from Neewer.
    Audio – Deity D3 or D3 Pro if you want audio dial control. If you want an external audio recorder I would opt for the Zoom H6, which you would feed the line out into audio input of the Z Cam for a scratch track and sync the audio from the recorder in post.
    Rig & Supports – Dual rosette hand grip mount, a pair of extension arms, 15mm rods with connectors, quick release for rapid transition to a tripod, offset 15mm rod shoulder mount and a counter weight. For gimbal use the Zhiyun Crane S3 has a 6.5KG payload, easily enough for a rigged out flagship.
    Tripod – Cayer fluid head tripod with carbon fiber legs – uses the same mounting base plate as the shoulder rig.


#### Sample Z Cam E2 S6 Kit


#### Sample Z Cam E2 M4 Kit


#### Sample Z Cam E2 Kit


<!-- This rig is from community member Boyan Ortse from Epic Pixel. -->



    Camera – Z Cam E2
    Cage – SmallRig cage for E2 (2264)
    Lens – Sigma Art 18-35 f/1.8 with PolarPro Variable ND Filter
    Right Handle – RVLVR Labs Clutch Handle
    Monitor – Atomos Ninja V with 1TB SSD, mounted with a SmallRig swivel monitor (2174), ontop of a SmallRig Cinematic Top Handle (2393)
    Recording Media – The one modification I would make to this rig is to put the mSata drive from the Samsung T5 SSD into a SolidPod Slim from NKI for major improvements to recording stability from the T5. That will fit in the same SmallRig SSD Holder (2174)



#### Sample Z Cam E2 Multicam Livestreaming Kit



