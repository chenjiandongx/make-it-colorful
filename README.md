# 使用卷积神经网络给图片上色

### 概述

本项目使用了 [siggraph2016_colorization](http://hi.cs.waseda.ac.jp/~iizuka/projects/colorization/en/) 一个基于卷积神经网络的图片自动上色模型。我觉得这个想法很赞，就收集一些历史老照片来重新上色看看会是怎样的。图片来源于网络。具体使用方法参考 [官方文档](https://github.com/satoshiiizuka/siggraph2016_colorization)。


### 初体验

我想下面这张图片大家都应该跟熟悉，Windows 系统的经典壁纸。这是原图。
<div align="center">
    <img src="images/windows_xp_origin.jpg">
</div>

去色后的效果。
<div align="center">
    <img src="images/input/windows_xp_input.jpg">
</div>

自动上色后的效果。
<div align="center">
    <img src="images/output/windows_xp_out.png">
</div>
效果可以说是非常棒了，基本上没有什么违和感！

### 画展

亚伯拉罕·林肯。亚历山大加德纳拍摄于 1865 年 2月
<div align="center">
    <img src="images/input/01.jpg">
    <img src="images/output/01_out.png">
</div>

在《纽约号》甲板上的拳击赛。1899 年 7 月 3 日。
<div align="center">
    <img src="images/input/02.jpg">
    <img src="images/output/02_out.png">
</div>

德国塞恩·维特根斯坦·塞恩（Sayn-Wittgenstein-Sayn）伯爵的子女，伊冯娜（13岁）和亚历山大（12岁）兄妹，在西班牙马略卡岛（Majorca）附近的游艇上饮料和抽烟。1955 年。
<div align="center">
    <img src="images/input/03.jpg">
    <img src="images/output/03_out.png">
</div>

一名欧及布威族（Ojibwe）原住民用鱼叉抓鱼。1908 年，在美国明尼苏达州。
<div align="center">
    <img src="images/input/04.jpg">
    <img src="images/output/04_out.png">
</div>

希特勒，与墨索里尼的女婿齐亚诺（Count Galeazzo Ciano，站在希特勒之右）和外交部长里宾特洛甫（Joachim von Ribbentrop），参加纳粹党（NSDAP）的一场会议。约1930 年。
<div align="center">
    <img src="images/input/05.jpg">
    <img src="images/output/05_out.png">
</div>

战士戴着防毒面具，在剥洋葱。1941 年 10 月 15 日，利比亚的托布鲁克（Tobruk）。
<div align="center">
    <img src="images/input/06.jpg">
    <img src="images/output/06_out.png">
</div>

足球明星杨（Walter Waddy Young）和他的队员在他们彩绘的 B-29 轰炸机前。1944 年 11 月 24 日。
<div align="center">
    <img src="images/input/07.jpg">
    <img src="images/output/07_out.png">
</div>

英国纹身艺术家乔治·伯切特。1930 年于加利福尼亚州。
<div align="center">
    <img src="images/input/08.jpg">
    <img src="images/output/08_out.png">
</div>

邮政人员在展示最新的电动车“Autopeds”。1917年，美国华盛顿特区。
<div align="center">
    <img src="images/input/09.jpg">
    <img src="images/output/09_out.png">
</div>

美国爵士歌手萨拉·沃恩（Sarah Vaughan）。约 1946 年。
<div align="center">
    <img src="images/input/10.jpg">
    <img src="images/output/10_out.png">
</div>

新英格兰的冠军诱饵制造商，乔·林肯。1926 年。
<div align="center">
    <img src="images/input/11.jpg">
    <img src="images/output/11_out.png">
</div>

在美国内战期间，一名士兵站在一辆运送加农砲的载具旁。1865 年左右，维吉尼亚州，楚利断崖（Drewry’s Bluff）
<div align="center">
    <img src="images/input/12.jpg">
    <img src="images/output/12_out.png">
</div>

一个母亲帮助孩子从有轨电车上下来。纽约百老汇，1913 年 7月。
<div align="center">
    <img src="images/input/13.jpg">
    <img src="images/output/13_out.png">
</div>

黑人在俄克拉荷马城的有轨电车上喝水。1939 年 7 月。
<div align="center">
    <img src="images/input/14.jpg">
    <img src="images/output/14_out.png">
</div>

约翰·肯尼迪（John F. Kennedy）从哈佛大学毕业时。1940 年夏天。
<div align="center">
    <img src="images/input/15.jpg">
    <img src="images/output/15_out.png">
</div>

纽约时代广场，1944 年。
<div align="center">
    <img src="images/input/16.jpg">
    <img src="images/output/16_out.png">
</div>

美军砲兵观测兵在硫磺岛上。1945 年 2 月。
<div align="center">
    <img src="images/input/17.jpg">
    <img src="images/output/17_out.png">
</div>

在明斯克（Minsk）的孩子们看着邻居被轰炸。这次轰炸是纳粹德国入侵苏俄的「巴巴罗萨行动」（Operation Barbarossa）中的一部分。1941年6月，白俄罗斯。
<div align="center">
    <img src="images/input/18.jpg">
    <img src="images/output/18_out.png">
</div>

斯大林和丘吉尔在雅尔塔会议期间。1945 年 2 月。
<div align="center">
    <img src="images/input/19.jpg">
    <img src="images/output/19_out.png">
</div>

爵士歌星路易斯·阿姆斯特朗（Lucille Armstrong）和露西尔（Lucille）在埃及狮身人面像前。1961 年 1 月 28 日。
<div align="center">
    <img src="images/input/20.jpg">
    <img src="images/output/20_out.png">
</div>

约瑟夫·戈培尔在发现摄影师阿尔弗雷德·艾森斯塔德是犹太人后对其怒目而视。1933 年。
<div align="center">
    <img src="images/input/21.jpg">
    <img src="images/output/21_out.png">
</div>

从国会大厦看田纳西州首府那什维尔。内战期间，1864 年。
<div align="center">
    <img src="images/input/22.jpg">
    <img src="images/output/22_out.png">
</div>

失业的木匠。1939 年、
<div align="center">
    <img src="images/input/23.jpg">
    <img src="images/output/23_out.png">
</div>

杰伊·麦尼利在奥林匹克礼堂人群中掀起了热潮。洛杉矶，1953 年。
<div align="center">
    <img src="images/input/24.jpg">
    <img src="images/output/24_out.png">
</div>

W.H.墨菲和他的同事展示他们的防弹背心。1923 年 10 月 13 日。
<div align="center">
    <img src="images/input/25.jpg">
    <img src="images/output/25_out.png">
</div>

著名诗人沃尔特·惠特曼。1887 年。
<div align="center">
    <img src="images/input/26.jpg">
    <img src="images/output/26_out.png">
</div>

伊丽莎白·泰勒。1956 年电影 'Giant'。
<div align="center">
    <img src="images/input/27.jpg">
    <img src="images/output/27_out.png">
</div>

被遗弃的男孩抱着他的毛绒玩具动物。伦敦，1945 年。
<div align="center">
    <img src="images/input/28.jpg">
    <img src="images/output/28_out.png">
</div>

汽车残骸。华盛顿，1921 年。
<div align="center">
    <img src="images/input/29.jpg">
    <img src="images/output/29_out.png">
</div>

巴尔的摩贫民窟地区的一个年轻男孩。1938 年 7 月。
<div align="center">
    <img src="images/input/30.jpg">
    <img src="images/output/30_out.png">
</div>


### 引用
```
 @Article{IizukaSIGGRAPH2016,
   author = {Satoshi Iizuka and Edgar Simo-Serra and Hiroshi Ishikawa},
   title = {{
       Let there be Color!: Joint End-to-end Learning of Global and Local 
       Image Priors for Automatic Image Colorization with Simultaneous Classification
       }},
   journal = "ACM Transactions on Graphics (Proc. of SIGGRAPH 2016)",
   year = 2016,
   volume = 35,
   number = 4,
 }
 ```


### License

MIT [©chenjiandongx](https://github.com/chenjiandongx)
