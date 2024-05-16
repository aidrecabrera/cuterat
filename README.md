# cuterat

![image](https://github.com/aidrecabrera/cuterat/assets/61798731/0e6e3025-a351-4acb-8f64-488b57d66399)

| Condition               | Time      |
|-------------------------|-----------|
| Light, no obstacle      | 9 minutes |
| No light, no obstacle   | 9 minutes |
| Light, with obstacle    | 9 minutes |
| No light, with obstacle | 9 minutes |


light no obstacle:
![image](https://github.com/aidrecabrera/cuterat/assets/61798731/7617d45e-0439-4cea-b0c1-d024fce7e772)
`libcamera-vid -t 360000 -o "rat_$(date +"%Y%m%d_%H%M%S").h264" --qt-preview --framerate 60 --tuning-file /usr/share/libcamera/ipa/rpi/vc4/imx219.json --width 1920 --height 1080`

no light no obstacle: 
![image](https://github.com/aidrecabrera/cuterat/assets/61798731/30b86188-42a5-412f-9163-70197cea7034)
`libcamera-vid -t 360000 -o "rat_$(date +"%Y%m%d_%H%M%S").h264" --qt-preview --framerate 60 --tuning-file /usr/share/libcamera/ipa/rpi/vc4/imx219_noir.json --width 1920 --height 1080 --shutter 5000 --analoggain 32 --awb auto --awbgains 0,0 --denoise cdn_hq`

