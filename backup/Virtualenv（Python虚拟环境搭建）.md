### 安装virtualenv
virtualenv是一个Python包，我们采用pip(Python的包管理器)来安装。假设我们已经安装好了pip，就可以使用pip来安装我们所需要的包。
```shell
$ pip install virtualenv
```
### 创建Python虚拟环境
利用 virtualenv [虚拟环境名称] 来创建虚拟Python环境，在虚拟环境里用pip安装的包都会安装到当前的虚拟环境中。
```bash
$ virtualenv .venv
```
如果系统里安装了不同的Python版本，可以使用--python来指定虚拟环境的python版本。

```bash
$ virtualenv --python /usr/local/webserver/python3.6/bin/python3.6 .venv
```
默认情况下虚拟环境不会依赖系统环境的site-packages，如果想依赖系统环境的site-packages，可以使用--system-site-packages来设置。

```bash
$ virtualenv --system-site-packages .venv
```
### 启动和退出虚拟环境
启动虚拟环境：activate
```bash
[...]$ source .venv/bin/activate
(.venv)[...]$

# 激活Virtualenv虚拟环境
source ./.venv/bin/activate
```
退出虚拟环境：deactivate

```bash
(.venv)[...]$ deactivate
[...]$
```
