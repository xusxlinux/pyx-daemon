#### 需要安装开发工具包
> [root@aliyun-zjk-node ~]# yum group install  "base" "Development tools" -y
#### 下载python3.6的源码包
> [root@aliyun-zjk-node ~]# wget https://www.python.org/ftp/python/3.6.5/Python-3.6.5.tgz


> tar xf Python-3.6.5.tgz
> cd Python-3.6.5/

> ./configure --prefix=/usr/local/python36
> make
> make altinstall


> ln -vs /usr/local/python36/bin/python3.6 /usr/local/bin/python36

> ln -vs /usr/local/python36/bin/pip3.6 /usr/local/bin/pip36

> vim /usr/bin/yum
> #!/usr/bin/python2.7

