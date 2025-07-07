# DLNA_DMR_XIAODU
 dlna_dmr for xiaodu
 
 
此版本请使用homeassistant 2025.4以后的版本\
官方的DLNA_DMR修改后适配小度音箱，由于小度音箱每次启动UUID会变动，这里以xml地址为准。\
解决小度不能自动停止需要每次点两次TTS才能发声的问题。\
支持小讯R1音箱安装app常开dlna的TTS。（官方原版只能支持开启蓝牙的内置dlna）。\
其它设备按官方原版DLNA_DMR不变。

同官方集成一样支持跨网段使用，配置时不选择直接提交，手动输入xml网址。

小度音箱： http://小度音箱IP:49494/description.xml

R1音箱安装R1-dlna.apk后 ： http://R1音箱IP:38520/description.xml

修复小度音箱不能正常播放TTS的问题，由于ha2025.4后TTS变成实时流输出，发声更及时，但小度就会一卡一卡永远播放不完。于是改成等流完成后复制成文件链接给小度播放。对于长文字内容会比较明显延迟，不好用还是比不能用要好吧。限定30秒内TTS生成完成才有效。
R1音箱等其它DLNA设备保持原TTS链接。


