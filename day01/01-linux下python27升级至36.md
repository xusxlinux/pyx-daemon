#### 需要安装开发工具包
> yum group install  "base" "Development tools" -y
#### 下载python3.6的源码包
> wget https://www.python.org/ftp/python/3.6.5/Python-3.6.5.tgz
#### 解压包
> tar xf Python-3.6.5.tgz
#### 进入该目录
> cd Python-3.6.5/
#### 编译
> ./configure --prefix=/usr/local/python36
#### 使用altinstall是python的安装方式
> make

> make altinstall
#### 创建python36软连接
> ln -vs /usr/local/python36/bin/python3.6 /usr/local/bin/python36
#### 创建pip36软连接
> ln -vs /usr/local/python36/bin/pip3.6 /usr/local/bin/pip36
#### 要使用yum命令需要的是pip2.7版本
```
vim /usr/bin/yum
#!/usr/bin/python2.7
```
