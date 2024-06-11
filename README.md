# Install-Image-rasbperrypi
To install a Yocto-built image on a Raspberry Pi SD card
## Steps 
 - Dont forget to but this line ```ENABLE_UART = "1"``` in ```local.conf```
 - Use ``` sudo apt install gnome-disk-utility``` to install Disks gnome
 - Connect ur sdcard open Disks                                                                                                                                    
 - be carefull choose the SD card
 - Choose format
   
   ![image](https://github.com/Rabie45/Install-Image-rasbperrypi/assets/76526170/f700b84a-3eb6-4162-8b99-7978e72278ad)
   ![image](https://github.com/Rabie45/Install-Image-rasbperrypi/assets/76526170/368def16-eb2b-46c6-ae95-64a639043d8b)
   
 - Press on ```+``` button
  ![image](https://github.com/Rabie45/Install-Image-rasbperrypi/assets/76526170/c1f2ff42-a01c-4327-bb31-c9915cf968f6)
  ![image](https://github.com/Rabie45/Install-Image-rasbperrypi/assets/76526170/ee5b7096-9456-4f4d-a1cd-412573ebcd3b)
  ![image](https://github.com/Rabie45/Install-Image-rasbperrypi/assets/76526170/117c8d39-d7ba-40a0-897f-c3837007976b)

 - Choose the sceond one
   ![image](https://github.com/Rabie45/Install-Image-rasbperrypi/assets/76526170/e35ff476-69b8-4187-9ac2-276b528d72a5)
   
 - Copy the wic file got from poky to build directory ```cp PATH/build/tmp/deploy/images/raspberrypi3/diploma-minimal-raspberrypi3.wic.bz2 .```
 - Unzip the file ``` bzip2 -dk diploma-minimal-raspberrypi3.wic.bz2```
 - The 'dd' command reads input from a file or a device, and writes it to another file or device. ```sudo dd if=diploma-minimal-raspberrypi3.wic of=/dev/sdc status=progress```
   ![image](https://github.com/Rabie45/Install-Image-rasbperrypi/assets/76526170/287a581d-1df4-43fd-af6e-7e30504997eb)
   
 - Remove ur sd to rasbperrypi
 - Connect ur ttl to usb with rasbperry pi
   ![image](https://github.com/Rabie45/Install-Image-rasbperrypi/assets/76526170/3fed1032-450e-4f02-9ee2-3cd9c5ca9db0)
   
 - TTL RX -> rasbperry TX
 - TTL TX -> rasbperry RX
 - GND -> GND
   ![image](https://github.com/Rabie45/Install-Image-rasbperrypi/assets/76526170/b2aa08d3-c045-4b6d-9120-449a044294ab)
   
 - Conect to usb and power on rasbperry pi


https://github.com/Rabie45/Install-Image-rasbperrypi/assets/76526170/bd074e36-576c-40b2-8750-7c159a1efe80




   







 
