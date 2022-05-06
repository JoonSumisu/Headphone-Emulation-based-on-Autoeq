# Headphone-Emulation-based-on-Autoeq

# 简介
本项目为基于Autoeq的算法，模拟其他耳机频响曲线的测试项目

Autoeq [GitHub Pages](https://github.com/jaakkopasanen/AutoEq)

如果有更高效的算法请大佬们告知

# 注意事项
仅供eq研究学习，听歌换口味，寻找失落的声音，想要买某个耳机先试听一下，没钱买某特贵的耳机就听个响，等等奇怪目的使用

使用eq数据后无法还原原版耳机的音色和soundstage，声音仅供参考

何为音色？ 

请参考：https://zh.m.wikipedia.org/zh-hans/%E9%9F%B3%E8%89%B2

何为soundstage？ 

文字解释 https://www.rtings.com/headphones/tests/sound-quality/passive-soundstage 

视频解释 https://www.youtube.com/watch?v=u2jHbaGST_Q

# 目录

measurements -- 通过各种手段获得的耳机原始频响曲线，格式为： 耳机名+来源平台.csv

compensation -- 数据来源的理想曲线，Autoeq项目算法的必须品

result -- 通过优化+主观听音后的数据，格式为 #原始耳机 to #目标耳机 .csv ，带有对比图，可以看到还原到什么程度

Autoeq code sample -- 个人使用Autoeq的示范代码，详细方式请看： Autoeq [GitHub Pages](https://github.com/jaakkopasanen/AutoEq)

Autoeq format to Neutron -- 将Autoeq 的ParametricEQ 文字 格式改写成 neutron fc_presets.xml 可用格式的小脚本。尽管可以高效的改写，但是自动化程度不够高，还是需要自己手动输入特定的内容。 等我python水平更高之后会优化的（指现在是0。 

# 数据来源

1.  git clone https://github.com/jaakkopasanen/AutoEq.git

 在Autoeq项目中获得大量的原始测量数据和目标曲线数据

2.  https://www.woodenears.com/
 
 由于罗天龙测试的数据是不提供下载，且不提供付费下载。
 
 只可以使用 https://apps.automeris.io/wpd/ 进行半手工的打点以获得数据，精度在实际听感下在可以接受的范围。
 
 具体操作指南 https://medium.com/@jaakkopasanen/make-your-headphones-sound-supreme-1cbd567832a9


# 所用听音设备
现在使用的耳机为

1.德行 罗马尼亚产 Ord.No.508824 HD 600 （HD600 曲线还原之神！

2.水月雨 竹 （99买不到吃亏的好耳机

3.小米 无线降噪耳机3 pro （手机降价送的

朋友的设备：天龙的d5200，三星 buds plus 等等。

# EQ软件
全平台：

[Neutron Music Player](https://neutroncode.com/)

由于为了通过更小的增益压低失真，需要10个以上的filter，neutron是很好的选择

测试下最好用的播放器，自带Autoeq的补偿曲线，也可以通过上面的小脚本倒入多filter的eq，也可以写入其他大神写的补偿曲线，还能使用corssfeed模拟音箱的声场

加上现在win11，跟m1 mac都能按照手机应用了。 neutron可能是最优解

Andorid：

[Neutron Music Player](https://neutroncode.com/)

测试下最好用的播放器，自带Autoeq的补偿曲线，也可以通过上面的小脚本倒入多filter的eq，也可以写入其他大神写的补偿曲线，还能使用corssfeed模拟音箱的声场

缺点是需要付费，可以在华为的应用商店下载并且付费，不需要在Googleplay上面买

[Wavelet](https://pittvandewitt.github.io/Wavelet/)

轻量的全局eq软件，自带Autoeq的补偿曲线，最重要的是完全免费

缺点是导入只能导入Autoeq的GraphicEQ格式，在实际测量上高频部分会有点问题。

Windows：

[Equalizer APO ](https://equalizerapo.com/)

因该是最优解，功能最强的软件

但是我作为一个纯纯的mac人无福消受

Mac:

[eqmac](https://eqmac.app/)

因该是Mac的最优解，但是是月租形式的，我没买

# 现有问题

对于Autoeq的理解不够深，部分耳机无法很好的还原

另外Autoeq的算法无法限定模拟范围，导致了频响曲线的模拟不是很理想，希望能那天变强到改写原代码

