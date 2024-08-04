1、根据需要更新的内容把以下对应文件拷贝到SD卡：

 (1)、更新配置文件：robin_nano35_cfg.txt
 (2)、更新图片：    mks_pic
 (3)、更新字库：    mks_font
 (4)、更新TFT固件： Robin_nano35.bin
 (5)、更新Wifi固件：MksWifi.bin

2、V1.0.2 修改问题：
（1）、修正sd卡读取大容量卡时，偶尔出现数据读取不正常的bug，更好的兼容SD卡；
（2）、修正手动关机无效的bug
（3）、修正打印中按换料，标题栏显示不正常的bug；
（4）、修正外接驱动打印会斜的bug
（5）、修正手动调平时，移动速度太快的bug。

3、V1.0.3 修改问题：
（1）、修正当温度保护时间过长时，无法发M303调节温度的问题；
（2）、增加复古版、简约版这两种风格;
（3）、当配置文件中不使能 WIFI功能时，界面中WIFI按钮不显示出来；
（4）、关于里面的主板信息可以通过配置文件修改；
（5）、当有暂停或者断电，恢复打印时应预先挤出一段，不然可能会有缺料、断层的现象，挤出长度可以做       在配置文档里面设置；
（6）、增加两进一出功能，可配置；
（7）、在配置文件中增加屏幕翻转180度的功能（bootloader可翻转）
（8）、增加wifi扫描列表功能，可配置；
（9）、打印完成后，弹出对话框，显示打印已完成，所用时间多少，下面有"确定"和 "再打印一次"按键；
（10）、兼容3D_TOUCH功能；
（11）、增加屏幕唤醒功能，可配置；
（12）、修改bootloader，修复使用TB67S109驱动PWC关机不成功问题；
（13）、开放脉冲保持时间参数；
（14）、修正用3Dtouch做自动调平时，断电续打会悬空打印的问题；
（15）、断料检测为低电平触发时，断料后暂停在没有料的情况下后点恢复打印，会打印一段才停，没有提        示先装耗材；
（16）、设置为两进一出，在挤出界面将挤出头选为挤出头2，再在预热界面预热，无法设置预热温度；
（17）、去掉开关类型设置中的断料检测开关设置；
（18）、开启休眠模式后，休眠后打印界面中的预览模型图片不显示；
（19）、接了MKS PWC模块后打印完延时3分钟再关机,防止堵头（时间可配置)；
（20）、robin2主板，当z轴回零最大值（第一个z轴限位接zmax），启用双z限位时候，z2限位接的是xmax接        口。当z回零时候，z1限位触发时候，2个z轴会同时停止
（21）、增加暂停位置可选为无效项；
（22）、修改文件名超过30个字节按停止答应Z轴往回零反方向走的问题；

4、V1.0.4 修改问题：
（1）、修正最大温度不报错问题；
（2）、修正打印中读不到卡一直加热问题；

//////////////////////////////////////////////////////////////

1、According to the content that needs to be updated, copy the following file to the SD card:

 (1)、update the config file：robin_nano35_cfg.txt
 (2)、update images：         mks_pic
 (3)、update font：           mks_font
 (4)、update TFT firmware：   Robin_nano35.bin
 (5)、update Wifi firmware：  MksWifi.bin

2、V1.0.2 Modifications:
 (1)、Fix the bug that read Large capacity sd card data error sometimes.
 (2)、Fix bug with manual shutdown invalid.
 (3)、Fixed a problem in which the title bar displayed abnormally during printing.
 (4)、Fixed bug where external drive printing would be skewed.
 (5)、Fixed a bug where moving too fast when manually leveling.

3、Modifications in version V1.0.3:
（1）、Fix bug:When the temperature protection time is too long, the M303 cannot be adjusted.
（2）、Add two UI styles, retro and simple.
（3）、When the WIFI function is not enabled in the configuration file, the WIFI button in the        interface is not displayed.
（4）、The information about the motherboard inside can be modified by the configuration file.
（5）、When there is a pause or power failure, the printing should be pre-extruded for a period        of time. Otherwise, there may be a shortage of material and a fault. The extrusion              length can be set in the configuration document.
（6）、Add two in one out function, configurable.
（7）、Increase the screen flip 180 degrees in the configuration file (bootloader can be               flipped).
（8）、Add wifi scan list function, configurable.
（9）、After the printing is completed, a dialog box will pop up to show that the printing has         been completed. How long does it take? There are "OK" and "Reprint once" buttons.
（10）、Compatible with 3D_TOUCH function.
（11）、Increase screen wake-up function, configurable.
（12）、Modify the bootloader, fix the failure to use the TB67S109 driver PWC shutdown.
（13）、Open pulse hold time parameter.
（14）、Fixed the problem that when using 3Dtouch to do automatic leveling, the power failure           will continue to print.
（15）、Fix bug:When the material detection is triggered by a low level, after the material is          cut off, the paper will resume printing after the material is not in use, and the                printing will be stopped after a period of time, without prompting to install the               consumables first.
（16）、Fix bug:Set to two in and one out, the extrusion head is selected as the extrusion head         2 at the extrusion interface, and then preheated at the preheating interface, the               preheating temperature cannot be set.
（17）、Fix bug:Remove the break detection switch setting in the switch type setting.
（18）、After the sleep mode is enabled, the preview model image in the print interface after           hibernation is not displayed;
（19）、After the MKS PWC module is connected, the delay is printed for 3 minutes and then              turned off to prevent plugging (time configurable).
（20）、Fix bug:When the z-axis returns to zero maximum (the first z-axis limit is connected to         zmax), when the double z limit is enabled, the z2 limit is connected to the xmax                interface.When z returns to zero, when the z1 limit is triggered, the two z axes will           stop at the same time.
（21）、Adding a pause position can be selected as an invalid item.
（22）、Modify the file name to exceed 30 bytes, and stop the problem that the Z axis is going          back to the zero direction.

4、V1.0.4 Modifications:
 (1)、Fixed the issue of maximum temperature not reporting errors.
 (2)、Fixed the problem that the nozzle is always heated during SD card read error.


