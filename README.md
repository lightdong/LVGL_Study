# LVGL_Study
模拟器环境的搭建：

lvgl官网：https://docs.lvgl.io/master/examples.html#size-styles

codeblocks下载：https://www.codeblocks.org/

解决edge浏览器，下载失败的问题：使用右键就可以解决

下载完整的lvgl“架构”与windows模拟器，
网址：https://github.com/lvgl/lv_port_win_codeblocks
在这个git里面可以选择自己想要的版本

可以自己建立learn.h & learn.c并在main函数中调用自己写的函数，用于学习各种小部件及设计自己的UI界面（如何想更进一步的话可以去学一下PS）

PS是个好东西

GUI是图形用户界面的意思，在生活中最常见的就是手机的触摸屏，用图形与触摸来实现人机的交互

GUI库就是用户可以自己根据别人已经写好的架构，在这个架构的基础上去调用API，这些API都是一些用于图形用户开发的库（比如说：按钮、菜单、下拉框）

现在来学习LVGL

LVGL的优点很广，也是现在势头正猛的一个GUI库

LVGL是完全免费且开源的，LVGL由C语言书写可以在任何的MCU | MPU上运行

LVGL提供了多种小部件功能，可以实现很漂亮的界面

v8.3

lv_conf.h中默认色深选择RGB565

/*Color depth: 1 (1 byte per pixel), 8 (RGB332), 16 (RGB565), 32 (ARGB8888)*/
#define LV_COLOR_DEPTH     16

main.c中选择模拟的屏幕分辨率为240*240

/*Initialize the HAL for LittlevGL*/
lv_win32_init(hInstance, SW_SHOWNORMAL, 240, 240, NULL);


打开编辑器后，字体可能会有点小

可以在setting -> editor -> font中进行修改font一般有字体的意思
![image](https://github.com/user-attachments/assets/24ec6161-4123-4871-997c-7de45ffb7489)

在下面可以修改配色&高亮的方案
![image](https://github.com/user-attachments/assets/5bb0da91-11f6-4795-b577-a6cecf1dbe05)



