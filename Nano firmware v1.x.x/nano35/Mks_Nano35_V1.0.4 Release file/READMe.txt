1��������Ҫ���µ����ݰ����¶�Ӧ�ļ�������SD����

 (1)�����������ļ���robin_nano35_cfg.txt
 (2)������ͼƬ��    mks_pic
 (3)�������ֿ⣺    mks_font
 (4)������TFT�̼��� Robin_nano35.bin
 (5)������Wifi�̼���MksWifi.bin

2��V1.0.2 �޸����⣺
��1��������sd����ȡ��������ʱ��ż���������ݶ�ȡ��������bug�����õļ���SD����
��2���������ֶ��ػ���Ч��bug
��3����������ӡ�а����ϣ���������ʾ��������bug��
��4�����������������ӡ��б��bug
��5���������ֶ���ƽʱ���ƶ��ٶ�̫���bug��

3��V1.0.3 �޸����⣺
��1�����������¶ȱ���ʱ�����ʱ���޷���M303�����¶ȵ����⣻
��2�������Ӹ��Ű桢��Լ�������ַ��;
��3�����������ļ��в�ʹ�� WIFI����ʱ��������WIFI��ť����ʾ������
��4�������������������Ϣ����ͨ�������ļ��޸ģ�
��5����������ͣ���߶ϵ磬�ָ���ӡʱӦԤ�ȼ���һ�Σ���Ȼ���ܻ���ȱ�ϡ��ϲ�����󣬼������ȿ�����       �������ĵ��������ã�
��6������������һ�����ܣ������ã�
��7�����������ļ���������Ļ��ת180�ȵĹ��ܣ�bootloader�ɷ�ת��
��8��������wifiɨ���б��ܣ������ã�
��9������ӡ��ɺ󣬵����Ի�����ʾ��ӡ����ɣ�����ʱ����٣�������"ȷ��"�� "�ٴ�ӡһ��"������
��10��������3D_TOUCH���ܣ�
��11����������Ļ���ѹ��ܣ������ã�
��12�����޸�bootloader���޸�ʹ��TB67S109����PWC�ػ����ɹ����⣻
��13�����������屣��ʱ�������
��14����������3Dtouch���Զ���ƽʱ���ϵ���������մ�ӡ�����⣻
��15�������ϼ��Ϊ�͵�ƽ����ʱ�����Ϻ���ͣ��û���ϵ�����º��ָ���ӡ�����ӡһ�β�ͣ��û����        ʾ��װ�Ĳģ�
��16��������Ϊ����һ�����ڼ������潫����ͷѡΪ����ͷ2������Ԥ�Ƚ���Ԥ�ȣ��޷�����Ԥ���¶ȣ�
��17����ȥ���������������еĶ��ϼ�⿪�����ã�
��18������������ģʽ�����ߺ��ӡ�����е�Ԥ��ģ��ͼƬ����ʾ��
��19��������MKS PWCģ����ӡ����ʱ3�����ٹػ�,��ֹ��ͷ��ʱ�������)��
��20����robin2���壬��z��������ֵ����һ��z����λ��zmax��������˫z��λʱ��z2��λ�ӵ���xmax��        �ڡ���z����ʱ��z1��λ����ʱ��2��z���ͬʱֹͣ
��21����������ͣλ�ÿ�ѡΪ��Ч�
��22�����޸��ļ�������30���ֽڰ�ֹͣ��ӦZ�������㷴�����ߵ����⣻

4��V1.0.4 �޸����⣺
��1������������¶Ȳ��������⣻
��2����������ӡ�ж�������һֱ�������⣻

//////////////////////////////////////////////////////////////

1��According to the content that needs to be updated, copy the following file to the SD card:

 (1)��update the config file��robin_nano35_cfg.txt
 (2)��update images��         mks_pic
 (3)��update font��           mks_font
 (4)��update TFT firmware��   Robin_nano35.bin
 (5)��update Wifi firmware��  MksWifi.bin

2��V1.0.2 Modifications:
 (1)��Fix the bug that read Large capacity sd card data error sometimes.
 (2)��Fix bug with manual shutdown invalid.
 (3)��Fixed a problem in which the title bar displayed abnormally during printing.
 (4)��Fixed bug where external drive printing would be skewed.
 (5)��Fixed a bug where moving too fast when manually leveling.

3��Modifications in version V1.0.3:
��1����Fix bug:When the temperature protection time is too long, the M303 cannot be adjusted.
��2����Add two UI styles, retro and simple.
��3����When the WIFI function is not enabled in the configuration file, the WIFI button in the        interface is not displayed.
��4����The information about the motherboard inside can be modified by the configuration file.
��5����When there is a pause or power failure, the printing should be pre-extruded for a period        of time. Otherwise, there may be a shortage of material and a fault. The extrusion              length can be set in the configuration document.
��6����Add two in one out function, configurable.
��7����Increase the screen flip 180 degrees in the configuration file (bootloader can be               flipped).
��8����Add wifi scan list function, configurable.
��9����After the printing is completed, a dialog box will pop up to show that the printing has         been completed. How long does it take? There are "OK" and "Reprint once" buttons.
��10����Compatible with 3D_TOUCH function.
��11����Increase screen wake-up function, configurable.
��12����Modify the bootloader, fix the failure to use the TB67S109 driver PWC shutdown.
��13����Open pulse hold time parameter.
��14����Fixed the problem that when using 3Dtouch to do automatic leveling, the power failure           will continue to print.
��15����Fix bug:When the material detection is triggered by a low level, after the material is          cut off, the paper will resume printing after the material is not in use, and the                printing will be stopped after a period of time, without prompting to install the               consumables first.
��16����Fix bug:Set to two in and one out, the extrusion head is selected as the extrusion head         2 at the extrusion interface, and then preheated at the preheating interface, the               preheating temperature cannot be set.
��17����Fix bug:Remove the break detection switch setting in the switch type setting.
��18����After the sleep mode is enabled, the preview model image in the print interface after           hibernation is not displayed;
��19����After the MKS PWC module is connected, the delay is printed for 3 minutes and then              turned off to prevent plugging (time configurable).
��20����Fix bug:When the z-axis returns to zero maximum (the first z-axis limit is connected to         zmax), when the double z limit is enabled, the z2 limit is connected to the xmax                interface.When z returns to zero, when the z1 limit is triggered, the two z axes will           stop at the same time.
��21����Adding a pause position can be selected as an invalid item.
��22����Modify the file name to exceed 30 bytes, and stop the problem that the Z axis is going          back to the zero direction.

4��V1.0.4 Modifications:
 (1)��Fixed the issue of maximum temperature not reporting errors.
 (2)��Fixed the problem that the nozzle is always heated during SD card read error.


