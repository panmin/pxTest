# pxTest
 android屏幕适配的两种方式：
 1. android官网上介绍了一种多屏幕适配的尺寸单位dp/dip
 > px = dp*(dpi/160)其中dpi是设备屏幕的密度，不同的设备dpi不同
    谷歌对dpi做了以下分类
    * ldpi ~120dpi
    * mdpi ~160dpi
    * hdpi ~240dpi
    * xhdpi ~320dpi
    * xxhdpi ~480dpi
    * xxxhdpi ~640dpi
    上述表述能够看出它是一个区间值，并不是固定的
    然而由于设备屏幕分辨率和屏幕密度并不是成一个固定的比例，所以全部用dp的写，似乎不是很好
 2. 使用px进行适配，本Demo就是此种方式
 > 现在常用的屏幕尺寸为1280x720,一般美工也会根据这个尺寸给图，图上标注的都是px，而android里面推荐使用的单位为dp，相同的屏幕尺寸，不同的密度比例，可能会要用到不同的dp值，这个转换很痛苦
  运行PxGenerator.java中的main方法就会生成对应的屏幕尺寸的px值