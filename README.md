# termux-quantaxis
![image](https://github.com/better319/termux-quantaxis/blob/master/pic/Screenshot_2018-07-27-08-02-06-590_com.termux.png)


termux-ubuntu安装：https://github.com/Neo-Oli/termux-ubuntu

apt-get install wget

apt-get install dos2unix

wget https://raw.githubusercontent.com/better319/termux-quantaxis/master/Installubuntu18.sh

dos2unix Installubuntu18.sh

bash Installubuntu18.sh

mongodb安装及启动

https://www.linuxidc.com/Linux/2018-05/152253.htm

apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5

echo "deb http://repo.mongodb.org/apt/ubuntu xenial/mongodb-org/3.6 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-3.6.list

apt-get update

apt-get install -y mongodb-org

cd /usr/bin/mongod

./mongod --dbpath /var/lib/mongodb/ --logpath /var/log/mongodb/mongodb.log --logappend &

mongo




然后进入/VAR/LIB/mongodb#mongo启动


-----------备用------

下面这个是正确步骤：

rm /var/lib/mongodb/mongod.lock

cd /usr/bin/

./mongod --dbpath /var/lib/mongodb/ --logpath /var/lib/mongodb/mongodb.log --logappend &

cd /var/lib/mongodb

mongo


然后进入/VAR/LIB/mongodb#mongo启动

---------------------------------


不要修改默认ubuntu的源

注意 python3 的utf-8编码的处理 
 
https://www.cnblogs.com/qhlblog/p/8622109.html

https://blog.csdn.net/paullinjie/article/details/52081747


在/home/.bash_profile 创建空白文件添加就行了
