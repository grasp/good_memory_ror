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


mongodb install
-------------------

git install
--------------------
