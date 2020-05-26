#### 安装软件
> pip3 install virtualenv

> pip3 install virtualenvwrapper

#### 设置环境变量
```
vim .bashrc
export VIRTUALENVWRAPPER_PYTHON=`which python3`               # 指定virtualenvwrapper执行的python版本
export VIRTUALENVWRAPPER_VIRTUALENV_ARGS='--no-site-packages' # 添加virtualenvwrapper的参数，生成干净隔绝的环境
export WORKON_HOME=/data/python-env                           # 指定虚拟环境存放目录，.virtualenvs目录名可自拟
export PROJECT_HOME=/data/python/project                      # 数据存放目录
source /usr/local/python36/bin/virtualenvwrapper.sh           # virtualenvwrapper.sh所在目录
```
#### 创建软连接
> ln -vs /usr/local/python36/bin/virtualenv /usr/bin/virtualenv
#### 创建虚拟环境
> mkvirtualenv py3-env
#### 可以指定py27或者py36
> mkvirtualenv --python=/usr/bin/python3 py3-env
#### 创建虚拟目录
> mkvirtualenv py3-env
#### 切换虚拟环境
> workon
#### 退出虚拟环境
> deactivate
#### 删除指定环境
> rmvirtualenv
#### 列出所有环境
> lsvirtualenv
#### 进入虚拟环境目录
> cdvirtualenv 
