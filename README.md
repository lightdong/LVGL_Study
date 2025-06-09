# LVGL_Study
模拟器环境的搭建：

lvgl官网：https://docs.lvgl.io/master/examples.html#size-styles

可以在官网中查看：各种的API、部件中有哪些枚举

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

左边的树不见了，怎么解决：shift + F2

下面的框不见了，怎么解决：

![image](https://github.com/user-attachments/assets/ad6afb4a-6a3a-46bf-963b-0d0bdb997694)

如何快速地查看颜色：
1.win+R mspaint可以打开windows自带的画板：
![image](https://github.com/user-attachments/assets/a3d005e3-decb-49ae-8ddd-aa4f6545e124)

2.在颜色提取器里面可以看到具体RGB斯格式：
![image](https://github.com/user-attachments/assets/7156060b-88cf-4068-b9dd-888057119b86)


可以在工程文件夹下添加自己的文件：

![image](https://github.com/user-attachments/assets/9c17cee4-2aa6-4e04-98fa-f92378c164d9)

在工程中添加文件夹后，就会有对应的.c与.h文件

![image](https://github.com/user-attachments/assets/a953fadf-8239-4051-9cb1-e92e70931ffe)

![image](https://github.com/user-attachments/assets/45ef506f-ab12-4a0e-bf42-1cc280607102)


在main.c可以像下面那样引入头文件：

![image](https://github.com/user-attachments/assets/310883d4-a617-41bd-9946-f294efc8ef51)


在lvgl中使用相应字体时，要开启相应的宏，字体相关的宏定义在lv_conf.h中

![image](https://github.com/user-attachments/assets/b143e5ff-d3a4-4f02-a1ca-cf75d8c27a11)

把宏定义修改为1即可

字体的信息存在相关的.c文件中
![image](https://github.com/user-attachments/assets/3f52b79d-453c-4a3a-aada-3398bd2a9b1e)

用下面的方法，可以设置UTF-8
![image](https://github.com/user-attachments/assets/78ffb420-2432-495d-bb34-cb74789c719e)


多行注释：ctrl+shift+c

多行取注注释：ctrl+shift+x












