# DLNA_DMR_XIAODU
 dlna_dmr for xiaodu
 
 
此版本请使用homeassistant 2023.1以后的版本\
官方的DLNA_DMR修改后适配小度音箱，由于小度音箱每次启动UUID会变动，这里以xml地址为准。\
解决小度不能自动停止需要每次点两次TTS才能发声的问题。\
支持小讯R1音箱安装app常开dlna的TTS。（官方原版只能支持开启蓝牙的内置dlna）。\
其它设备按官方原版DLNA_DMR不变。

同官方集成一样支持跨网段使用，配置时不选择直接提交，手动输入xml网址。

小度音箱： http://小度音箱IP:49494/description.xml

R1音箱安装R1-dlna.apk后 ： http://R1音箱IP:38520/description.xml


