---
id: 982
title: 智能家庭设计的一些想法
date: 2009-08-04T10:57:15+00:00
author: Eric
layout: post
guid: http://blog.youxu.info/?p=982
permalink: /2009/08/04/smarthome/
dsq_thread_id:
  - 337132976
categories:
  - Cool Stuff
  - Life
  - Linux
  - tech
---
以前我在博客里说过我用 Gtalk 控制我家的空调，这样我在回家之前就可以先开空调， 到家的时候正好家里凉爽起来了。 这个技术很简单， 只需要弄一个所谓的 X10 设备就行了。 我的朋友 Bao Sheng 做了一个[视频](http://forrestbao.blogspot.com/2008/09/control-your-home-appliance-thru.html)， 有兴趣的可以看看他的演示和讲解。

[以前我在博客里说过我用 Gtalk 控制我家的空调，这样我在回家之前就可以先开空调， 到家的时候正好家里凉爽起来了。 这个技术很简单， 只需要弄一个所谓的 X10 设备就行了。 我的朋友 Bao Sheng 做了一个[视频](http://forrestbao.blogspot.com/2008/09/control-your-home-appliance-thru.html)， 有兴趣的可以看看他的演示和讲解。

](http://en.wikipedia.org/wiki/X10_(industry_standard)) 是一种非常方便的协议， 所有的控制信号都通过家中的电源线传播， 所以设备一插到插座上， 就可以被控制，不需要另外布线， 即插即用，对于我这种租房的人来说非常方便。 X10 设备有很多控制的方式。 有一种 X10 设备， 可以连接在计算机上， 然后计算机就可以发送指令控制其他X10设备。 计算机和X10 之间的接口是串口，所以如果你觉得不爽，用单片机和一个 MAX232 芯片就可以控制了，不需要庞大的计算机。

如果家中的电灯等不是插在插座上，而是通过墙上开关控制，你只需要将家中原有的电灯开关换成支持 X10 的电灯开关就行了。这种 X10 的电灯开关， 和普通墙上开关大小一样，功能一样， 但在 eBay 上的售价比在 Home Depot 买的普通开关还便宜，所以完全可以把家中开关全部换掉。这样就可以用计算机控制家中原有的电灯。

空调， 电饭锅， 风扇， 电视机等电器都可以如此控制。 至于我说的网络控制，就更加简单了， Gtalk 协议都是公开的，只需要写个客户端挂机监听就行了。 如果想玩这套东西的， 我这里有源代码。 X10 还有无线射频接口, 所以可以在车上控制车库的门或者门口的灯， 在家也可以躺在床上一键关灯，都是无线接口能干的事情，这里面的技术，和电动车锁的原理是一样的，你甚至可以把家里面的锁换成车上那种，一有人撬，立即杀猪似的发出警报。

控制电器有很多应用， 比如看电影的时候，能够达到一键打开电视和DVD以及关掉大灯的效果。早晨也可以通过控制灯慢慢亮起来让人自然醒来。至于控制空调，电饭锅这些，都是完全看需要看想象力了。

以上这些玩意，属于第一代智能家庭，我家基本上都部署了。 我现在考虑把我们家往二代智能家庭进化， 具体来说要能做到以下几点， 有些技术细节我没想好， 所以写出来请各位读者大牛出主意。
  
**
  
1. 在计算机上可视化控制一切电器**

这个不难，只要写一个 GUI 客户端就行了。 如果想做得比较好玩一点，可以像  Second Life 一样， 把家中做成一个虚拟现实系统， 人走到哪个房间， 哪个房间灯自动点亮。 这个需要一个人的定位机制， 而且人身上的传感器要很小， 便于携带。 这个目前还没想好怎么弄。 大家帮我出出主意? 虚拟现实有什么好的软件? 是不是在门口装个摄像头做一下 Motion Detection 比较好？
  
**
  
2. 语音控制**

我想语音控制所有的家电。 我看到别人 hack 了一个无线对讲机，让这个对讲机的信号送到计算机里面，但是随身放一个对讲机好像太庞大了，目前正在考虑弄一个蓝牙耳机，这个蓝牙耳机和计算机连接起来，做语音识别，然后发送信号到家电。 计算机端的语音识别软件很多的，应该很好弄。
  
**
  
3. 大脑直接控制和其他控制**

BCI 技术还不成熟, 不过带一两个传感器的检测眼球运动的东西早就有了，如果要控制的东西不复杂，可以使用 [Ocz Nia](http://www.ocztechnology.com/products/ocz_peripherals/nia-neural_impulse_actuator)，  如果要复杂一点, 可以使用 [Emotiv](http://www.emotiv.com/). 唯一的不好就是要带个帽子到处走，倒没有一个随身的车钥匙大小的遥控器方便。 自从有了 WII, 我们可以 Hack 一个 WII Remote, 然后在家挥一下 WII Remote， 就可以让灯亮起来。 要是 WII Remote 再小一点，或者自己买一个加速传感器和位置传感器粘在筷子上， 就很有魔棒的感觉了，到时候对着灯一点，灯就亮了， 哈里波特保证拜你为师 :)
  
**
  
4. 传感器通信**

我家现在卧室的门上面都装了一个红外发射器（垃圾堆上捡了个电视遥控器，用了里面的红外发光二极管）和一个接收器，人进入屋子的时候会切断红外线一次，我就自动打开屋子里的灯，本来是贴在地上的， 可是我们家的猫老是走来走去，干扰系统，所以我不得不放在半人高的地方，可是这些器件总是要拖很长的线才能把信号送回去，我现在放半人高的地方，线拖下来， 猫就老在我接出去的线上面蹭痒，搞得系统三天两头挂掉。 各位知道有没有什么便宜的无线协议，能够把这些小器件之间的无线通信问题解决？ 市面上的 WIFI 传感器都要大几十美元一个，不够便宜，这些小器件走 X10 也不行，我家没那么多插口， 而且我还得投资 TTL 到 X10 的接口。 蓝牙和WIFI 模块都太贵，RF 技术我是白痴，而且也不知道怎么做一个不互相干扰的系统，各位有高人指点指点？

**5. 微型化计算机**

我最近找了一些不带风扇的，可以跑 Linux 的作为家庭媒体存储中心和控制中心的计算机， 我的要求是体积要小，耗能要低，可以放在客厅或者锁在锁在壁橱里面。 其实一个几十块钱的二手计算机就可以干这些事情了，但是噪音太大，长得难看，实在不适合放在客厅。

还有就是接口，至少要支持一些 USB 口，这样我外面才能接其他的外设。 我找了一顿没找到什么好的。 各位有什么建议? 我目前找到的包括 [WD My Book World Edition](http://www.wdc.com/en/products/products.asp?DriveID=586), 中科梦龙盒子（太贵）， [Foxboard](http://foxlx.acmesystems.it/), 和 [Marvell Plug Computer](http://www.marvell.com/products/embedded_processors/kirkwood/plugcomputer.jsp). 或者自己 DIY 一个 ATOM 芯片的机器, 或者买一个 ARM 开发版, 或者 Hack 一个  20 块钱的二手 TiVo. 我现在还在这些技术之间纠结，想要找性价比最好的。

同时我还想搞一块很节能的液晶面板，带触摸的，算是家庭控制中枢，可以看到所有的灯和传感器的工作情况，就是不知道有便宜的小触摸面板没有？

我的目标是建立一个智能的，让我安居乐业的家。 各位读着还有什么奇妙的想法?