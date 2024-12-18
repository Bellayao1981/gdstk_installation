# **步骤**

因为gdstk库依赖qhull和zlib库，所以我们需要先安装这两个库

安装qhull

```
unzip qhull-master.zip
cd qhull-master
cmake .
make
make install
```

安装zlib
```
tar -zxvf zlib-1.3.1.tar.gz
cd zlib-1.3.1
cmake .
make
make install
```
安装clipper
```
unzip gdstk-main.zip
cd gdstk-main
cd external
cmake .
make
make install
```
最后安装gdstk
```
cd ..
cmake -S . -B build
cmake --build build --target install
```

在c++代码编译时加上库文件路径

`-L/usr/local/lib -lgdstk -lclipper -lqhullcpp -lqhullstatic_r -lz`
