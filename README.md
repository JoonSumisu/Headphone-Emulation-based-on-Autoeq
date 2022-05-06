# Headphone-Emulation-based-on-Autoeq

# 简介
本项目为基于Autoeq的算法，模拟其他耳机频响曲线的测试项目

Autoeq [GitHub Pages](https://github.com/jaakkopasanen/AutoEq)

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

result -- 通过优化+主观听音后的数据，格式为 #原始耳机 to #目标耳机 .csv

Autoeq code sample -- 个人使用Autoeq的示范代码，详细方式请看： Autoeq [GitHub Pages](https://github.com/jaakkopasanen/AutoEq)

Autoeq format to Neutron -- 将Autoeq 

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
