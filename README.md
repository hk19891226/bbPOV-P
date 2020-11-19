# bbPOV-V3
A new milestone?  
![image](https://github.com/RealCorebb/bbPOV-V3/blob/main/IMG/logo.jpg)  
已有能用的，不过存不了多少数据，仓库地址：https://github.com/RealCorebb/bbPOV-V2  
需要完成的事情：  
1.更高密度的LED （自制PCB可解决，正在尝试）  
2.如何存储数据？当前使用ESP32芯片，可参考已有仓库，把所有帧数据都存到闪存里，但这样不能超过4M，所以信息很有限。所以在看有没有办法存到文件系统里，当画面到下一帧的时候再读取需要的数据。或者有没有更好的方法，总之要存更多的信息量。(现在发现NeopixelBus库可以直接读取BMP图像）  
3.一个APP提供上传图片、控制上下页。3D模型设计 （这些是最简单的了，不是什么问题）  

# 备选LED芯片
APA102-2020(好像有的版本IC芯片比较小，PWM速度不够)                          价格￥0.67  
HD107S-2020（查看了Datasheet，应该是无论5050还是2020版本都有着27khz的PWM）   价格￥0.80  
LC8822-2020（有的地方说是26khz的PWM，但Datasheet里没看到，不清楚）           价格￥0.68  
LC8823-2020（规格跟HD107S相似，但找不到购买地址）
![image](https://github.com/RealCorebb/bbPOV-V3/blob/main/IMG/LED_Chips.jpg)  
