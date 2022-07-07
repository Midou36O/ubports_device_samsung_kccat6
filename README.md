# Ubuntu Touch port to the Samsung Galaxy S5 Plus (kccat6)

## Warning ! The port is not complete and a lot of problems could occur when using this.

### NOTE: This is a rough explanation of the install procedure, it will get improved soon.


- To install ubports:
  1. Download the `halium-boot.img` and `system.img`
  2. Get [halium-install](https://gitlab.com/JBBgameich/halium-install)
  3. Get a [rootfs image from ubuntu touch](https://ci.ubports.com/job/xenial-hybris-android9-rootfs-armhf/)
  4. Go into Download Mode and plug your device to your computer. 
  5. Now run `heimdall flash --BOOT /path/to/halium-boot.img --no-reboot` and reboot into TWRP.
  6. Go to TWRP (you know where to get that, right?) and connect your device to your computer.
  7. Run `./halium-install  -v -s -p ut /path/to/ubuntu-touch-android9-armhf.tar.gz /path/to/system.img`
  8. You may have some issues running halium-install. If you ever get an error related to passwd. [This tool can help you fix this](https://github.com/mikkeloscar/binfmt-manager).
  9. After doing the steps, congrats! You successfully installed UBPorts to your device.

## Known issues:
    - SIM Card don't get detected yet.
    - Unplugging the device makes it crash and reboot infinitely, so you'll have to keep the cable connected to a computer (this isn't called a phone anymore is it?)
    - Camera Used to work, but it broke again. Will fix later.
    - Even if the camera app works and shows the camera feed, the images you take don't go through.
    - Hardware playback don't work yet.
    - Music Player don't play anything yet.
    - Wifi works but be careful to not turn it off (i enabled wifi the dirty way). The option will disappear and a way to enable this would be to either reboot or run some commmands.
    
    
