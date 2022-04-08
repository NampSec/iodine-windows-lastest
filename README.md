# iodine-windows-lastest
windows binanry
the lastest windows version of iodine
### 注意windows 下安装的[tap-windows](http://build.openvpn.net/downloads/releases/tap-windows-9.9.2_3.exe) 必须为9.9.x版本

### 如何编译

#####   `git clone https://github.com/yarrick/iodine.git`

##### 由于没必要安装`unix2dos`所以建议注释掉Makefile中的[unix2dos](https://github.com/yarrick/iodine/blob/1df7d235f5e1650ff5a2a0cc8fee461ff9f0c106/Makefile#L61) `@unix2dos iodine-latest/*`

##### 安装mingw64和libz-mingw-w64-dev,libz-mingw-w64`apt install mingw64 libz-mingw-w64-dev libz-mingw-w64`

##### 将作者给出的[zlib](https://code.kryo.se/iodine/deps/zlib.zip
) 中bin目录中的zlib1.dll文件放入`/usr/x86_64-w64-mingw32/bin/zlib1.dll` 和 `/usr/i686-w64-mingw32/bin/zlib1.dll`(也可以自己编译最新版，见[此处](https://blog.csdn.net/sunsides/article/details/84546335))

###### `cd iodine && make iodine-latest-windows.zip`
