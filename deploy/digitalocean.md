##reset root password
## add user hunter
* useradd hunter -m -r
* adduser hunter sudo

## install vim
sudo apt-get install vim

## change ubuntu 12.04 source to 163.com
* http://blog.ubuntusoft.com/ubuntu-update-source.html

* sudo mv sources.list sources.list.old
* sudo vim sources.list

* copy list into file

* sudo apt-get update

 因为有一次发现ubuntu的源有时候安装的某些源有问题，更新成163的就可以，因为我习惯使用了
 
public key没有找到
http://blog.sina.com.cn/s/blog_6ce7b8a60100n5p4.html
sudo gpg –keyserver keyserver.ubuntu.com –recv 5BB92C09DB82666
sudo gpg –keyserver keyserver.ubuntu.com –recv 16126D3A3E5C1192 ，这个不行

##digitalocan使用问题
* 1. 发现512M的主机生不了， 没有给你snapshot的按钮，怀疑是他们出问题了
* 2. 安装论坛后，经常down机，原因是因为内存分配不够，unicorn直接退出
* 3. 无奈之下，只好用2cpu, 2G的服务了，考虑到论坛和推送服务测试的需求
* 

## 其他

部署的时候，需要把ruby-china 这个部署的文件夹以及下面的改为hunter所有

sudo chown -R hunter:hunter ruby-china

如果是root所有，会导致cap 远程部署失败
