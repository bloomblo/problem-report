# problem-report
problems during the work.
# **问题报告**
1.出现问题：
> error: C:\ci\opencv_1512688052760\work\modules\imgproc\src\color.cpp:11048: error: (-215) scn == 3 || scn == 4 in function cv::cvtColor
即由于linux与windows文件路径的差异导致无法找到文件所在地而使代码无法运行。

2.解决方法：
①将代码中的相对路径改为绝对路径。
如将Paprika.jpeg改为D:\\cvtest\\Paprika.jpeg。
②代码不变，将进程的当前文件夹改为自己电脑上图片所在的文件夹地址。

3.linux和win文件路径差异：
①在Unix/Linux中，路径的分隔采用正斜杠"/"，比如"/home/fzu"；而在Windows中，路径分隔采用反斜杠"\"，比如"D:\tools\eclipse"。

②windows下的路径经常会用双反斜杠来表示，不管解析引擎是否将反斜杠解析成转义字符，最终在内存中得到的都是"\"，因此写成"D:\\tools\\eclipse"是不会出问题的。

【链接到路径差异具体说明】（http://blog.sina.com.cn/s/blog_13fe28d370102wqki.html）

