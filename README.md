# ssvpn
shadowsocks
#haodongz@yeah.net

######
shadowsocks.json 

{
"server":"ip",
"port_password":{
     "8989":"xxx",
     },
"timeout":60,
"method":"aes-256-cfb",
"fast_open":false,
"workers":1
}

#######
install

1. https://pypi.python.org/pypi/shadowsocks

dowsocks 2.8.2
https://pypi.python.org/packages/02/1e/e3a5135255d06813aca6631da31768d44f63692480af3a1621818008eb4a/shadowsocks-2.8.2.tar.gz

Download
shadowsocks-2.8.2.tar.gz
A fast tunnel proxy that help you get through firewalls

  

A fast tunnel proxy that helps you bypass firewalls.

Server

Install
Debian / Ubuntu:

apt-get install python-pip
pip install shadowsocks
CentOS:

yum install python-setuptools && easy_install pip
pip install shadowsocks
Windows:

See Install Server on Windows

Usage
ssserver -p 443 -k password -m rc4-md5
To run in the background:

sudo ssserver -p 443 -k password -m rc4-md5 --user nobody -d start
To stop:

sudo ssserver -d stop
To check the log:

 sudo less /var/log/shadowsocks.log
 /usr/bin/ssserver   -c /etc/shadowsocks.json   启动
  nohup ssserver -c /etc/shadowsocks.json > /dev/null 2>&1 &  后台启动
