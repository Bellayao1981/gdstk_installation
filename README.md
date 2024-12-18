**步骤**

安装qhull

(```bash
unzip qhull-master.zip
cd qhull-master
cmake .
make
make install
''')

安装zlib
```
tar -zxvf zlib-1.3.1.tar.gz
cd zlib-1.3.1
cmake .
make
make install
```
安装gdstk

`unzip gdstk-main.zip`

`cd gdstk-main`

`cmake -S . -B build`

`cmake --build build --target install`

在c++代码编译时加上

`-L/usr/local/lib -lgdstk -lclipper -lqhullcpp -lqhullstatic_r -lz`

注意gdstk解压包中external/中的clipper也需要单独安装
