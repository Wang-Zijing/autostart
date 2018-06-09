
# autostart
set python program to start at boot
在 /home/pi/.config 下创建一个文件夹，名称为 autostart，并在该文件夹下创建一个xxx.desktop文件（文件名以.desktop结尾，前面可以自定义）。
打开xxx.desktop文件，把下面的内容复制进去：

[Desktop Entry]
Name=example

Comment=My Python Program

Exec=python /home/pi/example.py

Icon=/home/pi/example.png

Terminal=false

MultipleArgs=false

Type=Application

Categories=Application;Development;

StartupNotify=true

保存上述文件，然后重启树莓派。此时mycar.py程序应该已经启动了。
