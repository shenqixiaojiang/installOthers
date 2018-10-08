# Protobuf
[down *tar.gz from Here](https://github.com/google/protobuf/releases) <br>
1、解压，进入目录 <br>
2、
```
 ./configure --prefix=Your_Path
 make
 make check
 make install
 
 export PATH=Your_Path/bin:$PATH
 export LD_LIBRARY_PATH=Your_Path/lib:$LD_LIBRARY_PATH
```
# Boost
### 安装方式1--一直没安装成功，结果还是用的方式2（😅）
[down *tar.gz from Here](https://dl.bintray.com/boostorg/release/1.68.0/source/) <br>
[安装参考链接](https://www.cnblogs.com/oloroso/p/4632848.html)

### 安装方式2
```
yum install boost
yum install boost-devel
yum install boost-doc
```
# Linux服务器端安装Matlab（非root用户）
* 首先将下载好的iso文件打开，将里面的文件copy到某个目录下，打包成zip文件上传到服务器（这里使用的是[2018a版本](https://pan.baidu.com/s/1yBZP6SFSN8uSuAxFgBCykQ)）。
```
./install -mode silent -agreeToLicense yes -fileInstallationKey 09806-07443-53955-64350-21751-41297 -destinationFolder ~/matlab/2018a/2018amatlab/
```
* 安装完成后，将Crack/R2018a/bin文件夹复制到安装目录下，最后在安装目录下的bin文件夹下使用
```
./matlab -c ~/Matlab/matlab2018a/Crack/license_standalone.lic 
```
即可启动matlab。建议在bash文件中使用[alias](http://man.linuxde.net/alias)命令进行设置：
```
alias matlab="~/Matlab/2018a_matlab/bin/matlab -c ~/Crack/license_standalone.lic"
```
