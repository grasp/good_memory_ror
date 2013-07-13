##reset root password
## add user hunter
useradd hunter -m -r
adduser hunter sudo

## install vim
sudo apt-get install vim

## change ubuntu 12.04 source to 163.com
参考了http://blog.csdn.net/troy_cornelius/article/details/7678119

* sudo mv sources.list sources.list.old
* sudo vim sources.list

* copy list into file

* sudo apt-get update

 因为有一次发现ubuntu的源有时候安装的某些源有问题，更新成163的就可以，因为我习惯使用了
 


