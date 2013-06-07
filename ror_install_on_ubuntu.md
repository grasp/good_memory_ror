ROR_Install_On Ubuntu
=====================

basic information
---------------------
*Ubuntu 12.04.02 LTS desktop i386 version 
*chrome browser install
** 解决 chrome CPU 100% -sudo apt-get install m4 
http://www.robgolding.com/blog/2010/06/07/fixing-google-chromes-100-cpu-usage-on-ubuntu/
still in verify

*webqq for communication with parter
* chinese input using default installed, not bad
* need learn some shotcut for ubuntu
 ** ctrl+alt+T
 ** super

editor tools
-----------------
*sublime text2
sudo add-apt-repository ppa:webupd8team/sublime-text-2  
sudo apt-get update  

Shell代码  
sudo apt-get install sublime-text-2-beta  
or  
sudo apt-get install sublime-text-2-dev  


ruby install
-------------------

as ruby 2.0 and rails 4.0 is coming, so I try to use latest , not sure the price.

RVM install  guide
--------------
http://ruby-china.org/wiki/rvm-guide


rails install
-------------------
淘宝网做了rubygems 镜像。

首先替换sources

gem sources --remove http://rubygems.org/

gem sources -a http://ruby.taobao.org/

gem sources -l       #用来查看source list

请确保只有http://ruby.taobao.org/ 一个

然后就可以gem install rails --no-ri --no-rdoc

为什么要用--no-ri --no-rdoc 参数，因为加上去安装快，而且这两个也用不着

安装完毕后，使用rails -v 查看版本，如果你看到正确显示版本，恭喜你，可以下一步了。





memcache install
------------------
http://aliyador.iteye.com/blog/1124721

* sudo apt-get install memcached 

check mem service

tarting memcached: memcached.
hunter@hunter-ruby:~/ruby-china$ ps -ef |grep mem
memcache  3987     1  0 07:03 ?        00:00:00 /usr/bin/memcached -m 64 -p 11211 -u memcache -l 127.0.0.1
hunter    4005  3427  0 07:03 pts/2    00:00:00 grep --color=auto mem

Redis install
-------------------------
http://www.2cto.com/database/201304/203768.html

* sudo apt-get install redis-server
* 
Starting redis-server: redis-server.
hunter@hunter-ruby:~/ruby-china$ ps -ef |grep redis
redis     4458     1  0 07:07 ?        00:00:00 /usr/bin/redis-server /etc/redis/redis.conf
hunter    4479  3427  0 07:08 pts/2    00:00:00 grep --color=auto redis


check redis server is run

Mongodb Install
-------------------------
http://docs.mongodb.org/manual/tutorial/install-mongodb-on-ubuntu/
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv 7F0CEB10
Create a /etc/apt/sources.list.d/10gen.list file using the following command.

echo 'deb http://downloads-distro.mongodb.org/repo/ubuntu-upstart dist 10gen' | sudo tee /etc/apt/sources.list.d/10gen.list
Now issue the following command to reload your repository:

sudo apt-get update
Install Packages
Issue the following command to install the latest stable version of MongoDB:

sudo apt-get install mongodb-10gen

check mongodb service by 
hunter@hunter-ruby:~/ruby-china$ ps -ef |grep mongodb
mongodb   5105     1  0 07:23 ?        00:00:00 /usr/bin/mongod --config /etc/mongodb.conf
hunter    5139  3427  0 07:25 pts/2    00:00:00 grep --color=auto mongodb

Install Image Magic
------------------------------
sudo apt-get install libmagickwand-dev
sudo apt-get install imagemagick

When this command completes, you have successfully installed MongoDB! Continue for configuration and start-up suggestions.

install libpng-dev
------------------------
sudo apt-get install libpng-dev


Install git on ubuntu
-----------------------
https://www.digitalocean.com/community/articles/how-to-install-git-on-ubuntu-12-04
sudo apt-get git-core git


copy ruby-china from github
-------------------------------
git clone https://github.com/ruby-china/ruby-china

RVM use issue
--------------
[[ -s "$HOME/.rvm/scripts/rvm" ]] && . "$HOME/.rvm/scripts/rvm"

check setup.rb , and run each command
--------------------------------------

install nodejs to compile js
--------------------------------------
https://github.com/joyent/node/wiki/Installing-Node.js-via-package-manager
sudo apt-get update
sudo apt-get install python-software-properties python g++ make
sudo add-apt-repository ppa:chris-lea/node.js
sudo apt-get update
sudo apt-get install nodejs

It installs current stable Node on the current stable Ubuntu. Quantal (12.10) users may need to install the software-properties-common package 
for the add-apt-repository command to work: sudo apt-get install software-properties-common

As of Node.js v0.10.0, the nodejs package from Chris Lea's repo includes both npm and nodejs-dev.

There is a naming conflict with the node package (Amateur Packet Radio Node Program),
and the nodejs binary has been renamed from node to nodejs. You'll need to symlink /usr/bin/node to 
/usr/bin/nodejs or you could uninstall the Amateur Packet Radio Node Program to avoid that conflict.

