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

## Z CAM Official Resources

**Resources on Z Cam’s Github**

– [Basic Info](https://github.com/imaginevision/Z-Camera-Doc/blob/master/E2/intro.md “”)

– [How to Sync E2 Cinema Camera (M/I/S Explained)](https://github.com/imaginevision/Z-Camera-Doc/blob/master/E2/howto/E2%20Sync%20Cable%20-%20Quick%20User%20Guide.pdf)

– [How to sync Timecode on Z Cam E2 Cinema Camera](https://github.com/imaginevision/Z-Camera-Doc/blob/master/E2/howto/Z-CAM-E2-Synchronize-time-code-with-external-device.pdf)

– Communication Protocols

  – [HTTP on E2 and Flagships](https://github.com/imaginevision/Z-Camera-Doc/blob/master/E2/protocol/http.md)

  – [HTTP on Z Cam E1](https://github.com/imaginevision/Z-Camera-Doc/blob/master/E1/http.md)

  – [LANC on E2 – Uses Sony’s LANC Protocol](https://github.com/imaginevision/Z-Camera-Doc/blob/master/E2/protocol/lanc.md)

  – UART – [Commands](https://github.com/imaginevision/Z-Camera-Doc/blob/master/E2/protocol/uart/uart_command.md) – [db9 pin info ](https://github.com/imaginevision/Z-Camera-Doc/blob/master/E2/protocol/uart/db9_pin.md) – [Camera UART Pinout (Tx,Rx,5V, Ground)](https://github.com/imaginevision/Z-Camera-Doc/blob/master/E2/protocol/uart/ctrl_pin.jpg)

– 3D Models of Z Cams – [E2c](https://github.com/imaginevision/Z-Camera-Doc/raw/master/E2/design/E2C_3D.zip) – [E2](https://github.com/imaginevision/Z-Camera-Doc/raw/master/E2/design/E2_3D.zip) – [E2 M4](https://github.com/imaginevision/Z-Camera-Doc/raw/master/E2/design/E2-M4_3D.zip) – [E2 S6](https://github.com/imaginevision/Z-Camera-Doc/raw/master/E2/design/E2-S6_3D.zip)

**Resources on Z Cam’s Website**

– [E2C User Manual (up to Firmware 0.93)](https://drive.google.com/file/d/1ABLlbGBeXCJOu-rnCrjw1tevuDleDyoM/view “E2C”)

– [E2 User Manual (up to firmware 0.89)](http://www.z-cam.com/wp-content/uploads/2019/10/Z-CAM-E2-User-Manual-draft-v0.6-FW0.89-.pdf “E2”)

– [Flagship (M4, S6, F6, F8) User Manual (up to firmware 0.93)](http://www.z-cam.com/wp-content/uploads/2020/04/Z-CAM-E2-Flagship-Series-User-Manual-draft-v0.2-FW0.93-.pdf “Flagship”)

– [How to color calibrate a Z Cam – also fixes stuck/dead pixels](http://www.z-cam.com/wp-content/uploads/2020/07/Z-CAM-E2-Hot-Pixel-Calibration-v1.2_draft.pdf “How”)

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

| Camera  | Low Native ISO  |  High Native ISO |

| :———— | :————: | :————: |

| F8 & S6  | 400  | 1250  |

| F6  | 400  | 2500  |

| E2 & M4 WDR Off<br>E2 & M4 WDR on  | 500<br>250  | 2500<br>1250  |

|  E2G & S6G | 1250  | –  |

| E2c  |  800 | –  |

### How to Expose for Zlog

  – 1st read [Jason’s Medium Post](https://medium.com/@jasonzhang_22759/the-design-of-log-curve-20541efda7fe) on the LOG design curve.

    >  The main take away from Jason’s article can be found in [this Facebook Post ](https://redux.vip/wp-content/uploads/2020/08/zlog-info.png)

  – Next, familiarize yourself with the False Color Spectrum of Z CAMs

![Z CAM False Color](https://redux.vip/wp-content/uploads/2020/08/image-1601536446515.png)

  > As a general rule you want to make sure your image is free from orange, purple, and blue while in false color mode. The neon green is where you want to aim to get your middle grey exposure, as this leaves 7 stops above to deal with over exposure. All skin tone exposure values in the scene should fall between the neon green and yellow regions.

## Header 2

## More Header 2
