# problem-report
problems during the work.
# **问题报告**
1.出现问题：
> error: C:\ci\opencv_1512688052760\work\modules\imgproc\src\color.cpp:11048: error: (-215) scn == 3 || scn == 4 in function cv::cvtColor
即由于linux与windows文件路径的差异导致无法找到文件所在地而使代码无法运行。

2.解决方法：
①将代码中的相对路径改为绝对路径。
如将Paprika.jpeg改为D:\\cvtest\\Paprika.jpeg
②代码不变，将进程的当前文件夹改为自己电脑上图片所在的文件夹地址。
