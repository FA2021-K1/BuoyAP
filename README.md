# BuoyAP
An ubuntu server 20.04 bootable image for Raspberry Pi with Buoy configurations (Like Access Point , docker and so on). 

For now:-<br/>
Access Point : BuoyAP <br/>
Password : drone@12 <br/>
IP: 192.168.10.50<br/>
Web service: http://192.168.10.50/v1/data

Current Status:-<br/>
Access point working<br/>
Docker working<br/>
Static IP working<br/>
Web service working<br/>

Should only work on 16gb or bigger SD cards for now. <br/><br/>

Link for the bootable img file:- <br/>
https://drive.google.com/file/d/1FYLWUSEJTA-4YVmJ91kznJR3f1rcvLRz/view?usp=sharing<br/>

flashing with Balena Etcher works. It might get stuck at 99%.<br/> 
Don't worry, just wait it will finish eventually.<br/>

If it is giving problems, extract the .gz file and flash the .img file.
Also delete the Android and LOST.DIR folder from the system-boot folder. Will fix that in the later release.<br/><br/>

Also, if you want to ssh it, use BuoyAP access point. (Password: raspberry, username: ubuntu)

path to netplan file: /etc/netplan/10-my-config.yaml<br/>
path to dtoverlay file: /boot/firmware/usercfg.txt<br/>

## Software used to make images
dd to make img file

PiShrink to shrink images to fit SD Cards. (https://github.com/Drewsif/PiShrink)

Gzip for compression

## Running the webservice on startup
To run the webservice that is prebuilt in the provided image on startup of the Raspberry Pi use the [systemd script](./systemd/buoy-web-service.service) provided in the systemd directory.
