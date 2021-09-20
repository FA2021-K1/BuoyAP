# BuoyAP
An ubuntu server 20.04 bootable image for Raspberry Pi with Buoy configurations (Like Access Point , docker and so on). 

For now:-<br/>
Access Point : BuoyAP <br/>
Password : drone@12 <br/><br/>

Current Status:-<br/>
Access point working<br/>
Docker working<br/>

Should only work on 16gb or bigger SD cards for now. <br/><br/>

Link for the bootable img file:- <br/>
https://drive.google.com/file/d/1No8VgwxtK12hOAy43CptYAd1jhNGOIve/view?usp=drivesdk <br/>

flashing with Balena Etcher works. It might get stuck at 99%.<br/> 
Don't worry, just wait it will finish eventually.<br/>

If it is giving problems, extract the .gz file and flash the .img file.
Also delete the Android and LOST.DIR folder from the system-boot folder. Will fix that in the later release.<br/><br/>

Also, if you want to ssh it, use LAN. Because Wifi will not work as it is being used for AP mode. (Password: raspberry)

path to file: /etc/netplan/10-my-config.yaml
