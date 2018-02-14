# axeldown-core

基于axel-webm的优化项目. 通过webui调用axel进行下载

## 使用方法

下载和编译:

``` bash
$ git clone https://github.com/lihaoyun6/axeldown-core.git
$ cd axeldown-core
$ chmod a+x build.sh
$ ./build.sh
```

环境准备:

因为项目基于web.py模块提供服务, 故需要先安装web.py

``` bash
$ easy_install web.py
```
在macOS等平台, 必要时请使用sudo安装 

``` bash
$ sudo easy_install web.py
```

启动运行:

``` bash
$ cd axeldown-core
$ python axeldown.py [自定义端口]
```
例如
``` bash
$ python axeldown.py 2333
```
(不使用自定义端口时, 默认在8080端口开启服务)

启动服务后在浏览器中打开"<http://127.0.0.1:端口>"即可看到管理界面

## 打赏

![image][data:image/png;base64,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]
