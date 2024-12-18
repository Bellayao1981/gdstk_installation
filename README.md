**安装步骤**
`unzip qhull-master.zip`
`cd qhull-master`
`cmake .`
`make`
`make install`

然后解压gdstk, 使用cmake生成makefile， make install安装

在编译时加上`-L/usr/local/lib -lgdstk -lclipper -lqhullcpp -lqhullstatic_r -lz`

注意gdstk解压包中external/中的clipper也需要单独安装
