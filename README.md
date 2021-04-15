# raspberry_pi_on_qemu
Rename the image file name after the option -sd (here 2021-01-11-raspios-buster-armhf.img) according to your downloaded image name
<pre>
"C:\Program Files\qemu\qemu-system-aarch64.exe" ^
-M raspi3b ^
-append "rw earlyprintk loglevel=8 console=ttyAMA0,115200 dwc_otg.lpm_enable=0 root=/dev/mmcblk0p2 rootdelay=1" ^
-dtb bcm2710-rpi-3-b-plus.dtb ^
-sd 2021-01-11-raspios-buster-armhf.img ^
-kernel kernel8.img ^
-m 1G ^
-smp 4 ^
-serial stdio ^
-usb ^
-device usb-mouse ^
-device usb-kbd ^
</pre>
