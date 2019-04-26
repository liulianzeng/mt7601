# MT7601
Linux driver for MT7601U with Monitor mode support and fixed memory leak

* support capture IPv4Multicast packet on Monitor mode
* support channel hopping on Monitor mode
* fixed memory leak on Monitor mode

源码中三个文件夹  依次为
* DPO_MT7601U_LinuxSTA_3.0.0.4_20130913 旧款源码 2.26.x及以前的代码 
* DPO_MT7601U_LinuxSTA_3.0.0.4_20130913_HI3518 旧款源码 2.26.x及以前的代码 
* mt7601u
以上两组源码中有提供对应的bin文件  需将对应的bin文件放入到对应的目录中
根据描述如下 cp ./DPO_MT7601U_LinuxSTA_3.0.0.4_20130913_HI3518/mcu/bin/MT7601.bin /lib/firmware/mt7601u.bin
而mt7601u的代码是从源码中扒下来的 4.2.x以上的代码中应该内置了对应的驱动代码,但是需要提供对应的bin文件才能正确使用
由于对应的github中的源码缺失  所以可以使用此源码中的代码和bin实现驱动
