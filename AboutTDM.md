# 介绍 #

TDM是一个类似于CDM的会话管理工具，是一个xinit扩展，利用它可以自己选择想要使用的桌面环境或zhcon,fbterm等工具。


# 用法 #

  * 首先禁用gdm,xdm等显示管理器
  * 假设TDM装在/usr/bin.安装后，请在~/.bash\_profile中写上source /usr/bin/tdm
  * 在~/.xinitrc或/etc/X11/xinit/xinitrc中去掉原有的打开窗口管理器的命令，改为exec tdm --xstart
  * 在~/.tdm/sessions/中加入打开窗口管理器或桌面环境的脚本，或指向相关可执行文件的链接
  * 在~/.tdm/extra/中加入非X11的程序，如zhcon,fbterm,weston等