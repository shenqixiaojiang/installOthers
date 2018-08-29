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
## 安装方式1--一直没安装成功，结果还是用的方式2（😅）
[down *tar.gz from Here](https://dl.bintray.com/boostorg/release/1.68.0/source/)
[参考链接](https://www.cnblogs.com/oloroso/p/4632848.html)

## 安装方式2
```
yum install boost
yum install boost-devel
yum install boost-doc
```
