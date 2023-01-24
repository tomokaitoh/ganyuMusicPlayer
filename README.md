# ganyuMusicPlayer
一个能在Windows控制台播放甘雨pv曲《梦里韶光》的简单程序。

# 编译说明
1. 在Visual Studio上编译的时候，需要在 `"项目"->"属性"->"C/C++"->"命令行"->"其他选项"` 中加入`/utf-8`,否则会出现乱码。
2. 如果出现编译错误`C2001:常量中有换行符`，需要在Visual Studio的**高级保存选项**中将编码改为`Unicode(UTF-8 带签名)-代码页65001`。
   
   打开**高级保存选项**的方法：
   工具 -> 自定义 -> 命令，在"菜单栏"项选择"文件"，点击"添加命令"，在"类别栏"中选择"文件"，在"命令栏"中找到"高级保存选项"，单击"确定"保存。在Viusal Studio主界面工具栏的"文件"中即可找到高级保存选项。
3. 用gcc编译器编译时需要链接vfw32库:

   `gcc ganyuMusicPlayer.c -o ganyuMusicPlayer.exe -lvfw32`

# 运行说明
1. 如果安装了Windows Terminal，程序运行在Windows Terminal中会出现颜色异常。可以在设置中将默认终端程序改为"Windows控制台主机",重新打开cmd，就是经典的Windows控制台了。
