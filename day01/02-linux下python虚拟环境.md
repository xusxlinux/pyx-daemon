#### 安装软件
> pip3 install virtualenv

> pip install virtualenvwrapper

#### 设置环境变量
```
vim .bashrc
export VIRTUALENVWRAPPER_PYTHON=`which python3`    # 指定virtualenvwrapper执行的python版本
export WORKON_HOME=/data/python/project/venv       # 指定虚拟环境存放目录，.virtualenvs目录名可自拟
export PROJECT_HOME=/data/python/project
source /usr/local/bin/virtualenvwrapper.sh         # virtualenvwrapper.sh所在目录
```
#### 创建软连接
> ln -vs /usr/local/python36/bin/virtualenv /usr/bin/virtualenv
