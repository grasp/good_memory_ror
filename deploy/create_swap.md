## reference
* http://wiki.ubuntu.org.cn/UbuntuHelp:SwapFaq

##main command and step 
* first create 5120M size file
** sudo dd if=/dev/zero of=/mnt/5120Mb.swap bs=1M count=5120

* formatting swap
sudo mkswap /mnt/5120Mb.swap

* adding swap to system
sudo swapon /mnt/5120Mb.swap

* check swap by 
cat /proc/meminfo

##add swap permantally
* Edit the /etc/fstab:
sudo vim  /etc/fstab

* Add this line at the end of the file:
/mnt/5120Mb.swap  none  swap  sw  0 0

* save and reboot machine
