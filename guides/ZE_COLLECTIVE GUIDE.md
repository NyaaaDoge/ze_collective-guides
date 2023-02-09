# CS:GO 僵尸逃跑地图 ze_collective 游玩指南

[![ze_collective_logo](images/ze_collective_logo.png)](http://luffaren.com/ze_collective.php)

Map core by [Luffaren](https://steamcommunity.com/id/LuffarenPer) (STEAM_1:1:22521282)  
This guide by [NyaaaDoge](https://steamcommunity.com/id/NyaaaDoge/) (STEAM_1:1:59449830)

----

## 1. 目录索引  

- [CS:GO 僵尸逃跑地图 ze\_collective 游玩指南](#csgo-僵尸逃跑地图-ze_collective-游玩指南)
  - [1. 目录索引](#1-目录索引)
  - [2. 前言](#2-前言)
  - [3. 地图基本说明](#3-地图基本说明)
    - [3.1 地图基本流程](#31-地图基本流程)
    - [3.2 关卡说明](#32-关卡说明)
      - [3.2.1 关卡难度](#321-关卡难度)
  - [4. 关卡结局](#4-关卡结局)
  - [5. 认识小地图中的基本色块](#5-认识小地图中的基本色块)
    - [5.1 起始与终点地块](#51-起始与终点地块)
    - [5.2 道路和地板色块](#52-道路和地板色块)
    - [5.3 物品色块](#53-物品色块)
    - [5.4 陷阱色块](#54-陷阱色块)
    - [5.5 其他常见的色块](#55-其他常见的色块)
    - [5.6 简单总结](#56-简单总结)
  - [6. 关卡主题](#6-关卡主题)
  - [7. 地图事件](#7-地图事件)
    - [7.1 事件刷新机制](#71-事件刷新机制)
    - [7.2 事件列表](#72-事件列表)
  - [8. 地图物品](#8-地图物品)
    - [8.1 (未翻译)人类物品 HUMAN (TEAM 3)](#81-未翻译人类物品-human-team-3)
    - [8.2 (未翻译)僵尸物品 ZOMBIE (TEAM 2)](#82-未翻译僵尸物品-zombie-team-2)
  - [9. 陷阱地块](#9-陷阱地块)
    - [9.1 Traps spawn](#91-traps-spawn)
    - [9.2 Traps vicinity](#92-traps-vicinity)
    - [9.3 Traps step](#93-traps-step)
  - [10. 一些小彩蛋](#10-一些小彩蛋)
  - [11. 写在最后](#11-写在最后)

----

## 2. 前言

![INTRO](images/INTRO.png)
  
CS:GO 僵尸逃跑[^僵尸逃跑模式]地图 ze_collective 是 Luffaren 创作内核、玩家创造大部分主要关卡的一张近似于随机生成的僵尸逃跑地图。你可以简单理解为ze中的 *Roguelike* 模式，地图流程都是基于随机生成的关卡进行的，该地图的运气成分还是挺重要的。此指南旨在介绍 ze_collective[^ze_collective] 的部分内容，便于玩家在地图中获得更好的游戏体验，同时激发有想法的玩家去使用[ze_collective关卡创作工具](http://www.luffaren.com/misc/PixelPaint/pixel-paint-master/index.php)去创造自己心目中的关卡。本指南目前只有一个人编写，如有错误请大胆指出，感激不尽。  
![CREATEMAP](images/CREATEYOURMAP.jpg)
  
**[前往Gamebanana下载该地图](https://gamebanana.com/mods/395733)**

[^僵尸逃跑模式]: 英文全称 Zombie Escape，主要的游玩方式就是人类需要使用尽可能多的手段阻止僵尸 感染/击破 人类，僵尸需要用各种方式阻止人类逃跑，包括但不限于 感染/击破 人类。人类躲避僵尸进行逃跑通常会有终点，一般情况下到达终点 躲避/消灭 所有僵尸即可获得游戏的胜利。
[^ze_collective]: 编写此指南的时候地图版本为v1_9，其中的`数值`可能会根据版本不同而改变。

## 3. 地图基本说明

### 3.1 地图基本流程

人类需要通过由各种小关卡组成的大关卡并且完成相应的结局，僵尸则需要使用各种手段阻挠人类达成胜利，被选为母体僵尸也有很多好处，请先不要着急。
  
人类需要在80s内触发每一个小关卡的终点，如果在60s内没有触发完成会让僵尸启用无敌。每一个小关卡都会在屏幕下方以一张20x20的像素图片minimap的形式出现，里面通常可以读出很多的地图信息，如果您是地图指挥建议请不要忽视该信息。如果想知道每个色块对应的东西可以前往[Luffaren的网站](http://luffaren.com/ze_collective.php)查阅相关信息[^查阅相关信息]。
  
每一大关都是由几个不同的小关卡和一个结局关卡(部分结局可能没有新生成关卡)组成的大关卡，
通常情况下会同时存在3个小关卡，最前面的关卡触发了，最后的关卡会在特定时间内逐渐消失（消失时间固定5s）。具体时间看是第几大关。在生成下一张地图的时候，会将上一张地图的开关、障碍物全部清除。  
通关普通Finale之后会开启无限模式(Infinite mode)[^开启无限模式]，你可以以通关为目标，也可以以游玩尽可能多的关卡为目标，总之，一切取决于玩家怎么想。

地图中的小关卡数不胜数并且会一直保持增长，也许其中会有你认识的人甚至是你自己创造的关卡呢？！  
![MAPLISTV19](images/SOMEMAPSART.jpg)  
  
[^查阅相关信息]: 绘画工具和每个色块说明请在[此处查阅](http://www.luffaren.com/misc/PixelPaint/pixel-paint-master/index.php)
[^开启无限模式]: 出生点上方就是调关房，noclip上去按按钮即可。
  
### 3.2 关卡说明

| 大关卡 | 小关卡（pixel-stages）数   | 说明 | 变黑圈到开始逐渐消失时间 |
| ---- | ---- | ---- | ---- |
| Level 1 | 5 (+1) stages | 可能+1结局关 | 关卡变黑圈5s开始逐渐消失(5s+5s)  |
| Level 2 | 6 (+1) stages | 可能+1结局关 | 关卡变黑圈8s开始逐渐消失(8s+5s)  |
| Level 3 | 7 (+1) stages | 可能+1结局关 | 关卡变黑圈10s开始逐渐消失(10s+5s) |
| Level 4 | 8 (+1) stages | 可能+1结局关 | 关卡变黑圈15s开始逐渐消失(15s+5s) |
| Finale  | 10 +1 stages | 先进行BOSS战后10关逃亡路。最后是 1 关是金字塔守点（守40s），倒计时25s会出现神风飞机 | 逃亡路关卡触发紫圈后3s最后的关卡快速消失 |
| Infinite mode | 想打多少打多少。10关后出现眼睛，射击其进行投票Checkout，通过后进入Boss战 | Boss之后的逃亡路有 10 + 当前地图池关卡的总数\*0.003（向下取整） stages（最多增加20关） | 普通关卡变黑圈10s开始逐渐消失(10s+5s)。逃亡路关卡触发紫圈后3s最后的关卡快速消失 |

#### 3.2.1 关卡难度

每一大关的难度都会有所不同，具体体现在每一大关的按钮触发时间、障碍物耐久、有害液体伤害、陷阱生成概率、事件刷新频率[^事件刷新频率]等。

| 关卡 | 事件刷新保底概率(%) | 关卡未触发事件增加概率(%) | 事件CD最大值(levels) | 延时门打开时间(sec) | 开关门打开用时(sec) | 障碍物耐久(倍) | 有害液体伤害 | 陷阱地块产生陷阱概率(%) | 初始ZM物品 |
|---|---|---|---|---|---|---|---|---|---|
| stage 1 | 15 | 5 | 5 | 2 | 0 | 0.5 | 4 | 20 | 2 |
| stage 2 | 20 | 5 | 4 | 4 | 2 | 0.75  | 9  | 40 | 3 |
| stage 3 | 25  | 5 | 3 |  6 | 4 | 1.0 | 14 | 60 | 4 |
| stage 4 | 30  | 10 | 3 | 8 | 6 | 1.5 | 19 | 80 | 5 |
| stage infinite| 15 | 5 | 5 | 5 | 0 | 0.8 | 9 | 30 | 5 |

由此可见 Infinite mode 并不一定是最难的，请广大玩家还不要畏惧这个模式，无限关的难度方面相对设计的比较舒适，可以多多尝试玩玩各种各样有趣华丽的关卡。  
[^事件刷新频率]: 事件刷新机制请前往 [7. 地图事件](#7-地图事件) 一节查看。

**Boss战**
![BOSSARENA](images/FINALEBOSSARENA.jpg)
Boss拥有基础血量3000，普通Finale每个人类增加血量17000。无限Finale每个人类增加20000，无限Finale也会地图池的关卡总数计算Boss血量，每个关卡增加30，以关卡增加血量的方式最多增加100000。每个人类在Boss战中阵亡会减少Boss 8000的血量。一颗雷对Boss造成2500伤害同时有30%几率击晕Boss 2s。
Boss直接触碰人类造成高额伤害，Boss有如下技能：

1. 直视人类的时候可能会发射蓝色光波将人类往Boss方向吸引，此时被吸引人可以不用看向Boss，躲避技能。
2. 用他的尾巴敲打人类
3. 拆除Boss战平台脚下的方块用来砸人
4. Boss固定，前摇散发黄色光波，释放推力将人类往外平台外推，人类视野里面没有Boss可以不被推力影响，往平台外看。
5. Boss到场地中央甩他的尾巴，人类跳低刀来躲避

| 关卡 | Boss数量（最多5只） | Boss血量 | Boss最大眩晕时间 |
| ---- | ---- | ---- | ---- |
| Finale | 1 只 | 3000 + CT人数*17000 + 当前地图池关卡的总数\*30（关卡增加的血量最多100000） | 20s |
| Infinite Finale | 2 + 当前地图池关卡的总数\*0.0004（向下取整） | 3000 + CT人数\*20000 + 当前地图池关卡的总数\*30（关卡增加的血量最多100000） | 10s |

人类也会根据地图池关卡的总数增加对应的伤害倍率。  
人类对Boss的伤害倍率 = 1.00 + 当前地图池关卡的总数\*0.0001（最多增加2.0） (无限关 + 0.50）

> 关于Finale：20s生成到电梯门口，15s电梯门开（4s开完），15s电梯门关（4s延迟门），再过15s电梯门开。进入低重力区域需要寻找各种平台往高处飞一直到最顶端的电梯上，可以一格一格跳，也可以一次跳两格。
![FINALELOWGRAV](images/FINALELOWGRA1.jpg)
> 等电梯上升后抬头躲天坠碎片。![DEBIRS](images/FINALERISING.jpg)电梯到顶10s后Boss苏醒且可被攻击，进入Boss战。普通Finale Boss打完Boss大概18s落地到第一个stage进行Finale Endrun。  
> 普通Finale Endrun会关闭Traps和Trap Floor的刷新，通常Endrun不会刷新大部分可交互元素，专心寻找逃亡路即可。逃亡路会一直有天坠掉落方块碎片，并且摔下虚空直接死亡，没有假摔机会。 一直到最后金字塔守40s，神风飞机会在触发金字塔后15s刷新（也就是倒计时30s）。电梯上升，僵尸死亡，人类胜利。  
>
> 关于Infinite模式下的Finale：Boss电梯上升的天坠伤害增加。逃亡路每一个stage都会刷zm神器，并且无限Finale Endrun会启用陷阱地块的陷阱刷新，同时固定每隔25s到50s之间随机选母体僵尸刷出神风飞机。同时也会刷其他事件。

## 4. 关卡结局

| 结局 | 说明 | 备注 |
| ---- | ---- | ---- |
| RISE | 往高处走守住最后的平台 | 路上的地板会分崩离析 |
| CLIMB | 往上爬守住最后的高台死守100s | 8.8s后跳板开放，结局35s后会有天坠，113s后高塔逐渐崩塌。结局36s后会无限刷新僵尸flight物品（固定5个），140s后处死所有僵尸flight |
| BUNKER | 守住最后的地堡90s直至没有僵尸剩余 | 60s后前面的关卡会全部消失。地结局堡垒的墙壁不会被毁灭大锤锤。僵尸进入地堡会变成1000hp，如果在外面全部坍塌40s后没能消灭僵尸将会全体处死 |
| BRIDGE | 结局守住最后的桥45s | 28s后前面的关卡全部消失 |
| ASCEND | 需要守住自己的地形60s后等待起飞，起飞12s后处死僵尸胜利 | 最后需要一块没有顶头的区域起飞到顶端。9s后会刷僵尸flight和僵尸moonboost|
| CONFLIT | 斯巴达结局人类守旗60s，僵尸占旗进度需要100% | 高跳需要按蹲之后再跳才能跳得高（可以蹲着跳）。战场上会刷各种物品。僵尸碰到人类会造成伤害，僵尸初始血量100，每个人类增加180hp |
| HUNT | 人类有65s的时间去猎杀僵尸 | 人类tp回起点只有在开头的5s有防抓免疫。僵尸基础血量150hp，每个人类增加25hp |
| RACE | 结局人类坐上卡丁车存活120s或者等到僵尸全部死掉 | 卡丁车操作是往水平方向向上看是加速，垂直水平方向看是正常速度，往下看是减速。（在非卡丁车结局中可以视角往最下面看下车，但是RACE结局锁了这个功能，同理非RACE结局情况下可以往最头上看跳跃）。天上会掉方块碎片，每块造成29点伤害。僵尸卡丁车碰到人类后会自爆。 |

## 5. 认识小地图中的基本色块

### 5.1 起始与终点地块

哥们随便抽一张minimap，你能读出其中的关键信息吗？  
![PIXELSTAGE](images/PIXEL-STAGE.png)  
它放到游戏里面是这样的  
![Turnabout](images/Turnabout.png)  

首先你需要了解 开始/结束 颜色地块。
它的颜色是这样![START_END](images/START_END_TILE.png)的，有了他你才能知道哪里是关卡的起点与终点。需要提及的一点就是，起点色块永远并且一定是在小地图的最左侧，你对小地图的阅读顺序应该是从左往右寻找给断后部队撤退的那条路。![START_END_REFERENCE](images/reference_start_end.png)  
如果关卡设置了结束按钮![ENDBUTTONTILE](images/ENDBUTTONTILE.png)，终点的圈会从默认的紫色（触碰即可触发终点）变成红色（需要按下所有紫色的按钮才能触发终点）  ![ENDRED](images/ENDBUTTON.png)  
按下这些紫色的按钮即可触发终点  
![ENDBUTTONS](images/ENDBUTTON2.png)

### 5.2 道路和地板色块

![COLORBASE](images/CORLORBASE.png)  
这些色块构成了绝大部分地图的路和地板。颜色越浅代表高度越高，同理越深越暗代表高度越低。白色代表普通地板，黄色代表平台地板，褐色代表普通地板上面有天花板（天花板其实是平台地板），红色代表普通地板头上是超高的墙壁。  
![FLOORREF](images/reference_floor.png)

### 5.3 物品色块

如想查看物品列表请查看 [8. 地图物品](#8-地图物品) 一节。  
人类神器物品刷新的色块![ITEMH](images/ITEMHUMAN.png)  
僵尸神器物品刷新的色块![ITEMZ](images/ITEMZM.png)  
![ITEMREF](images/reference_item.png)

### 5.4 陷阱色块

最后是陷阱刷新的色块![TRAPSTILE](images/TRAPSTILES.png)  
陷阱列表可以前往 [9. 陷阱地块](#9-陷阱地块) 一节查看。

### 5.5 其他常见的色块  

这些色块大部分的小地图都有使用到，同样是比较常见的色块。

1. 开关门色块![HOLD1](images/HOLD1.png)  
普通的开关门是绿色的色块。
前面两个色块分别是HOLD 1（门）、BUTTON 1（按钮）。后面的色块就是HOLD 2、BUTTON 2。以此类推，一共有4个开关门色块，只有按下所有对应的按钮才能开启这个开关门。  
![HOLDREF](images/reference_hold.png)
还有一种色块就是逆转开关门色块![HOLD2](images/HOLD2.png)。这些色块只有在按下了所有对应的按钮之后才会升起/关闭，平常状态下是开启/降下的。  
![HOLDIVH](images/reference_hold_inverted.png)

2. 传送入口与传送终点色块![TELEPORT1](images/TELEPORT1.png)![TELEPORT2](images/TELEPOR2.png)  
与开个关门色块类似，前面两个色块分别是TELEPORT 1（传送门入口）、TELEPORTDES 1（传送终点）。后面依次类推，一共有4个传送入口色块。  
需要注意的是，玩家有超过400的下降速度(从~+5的高度或以上跳落到传送门上)，它会让玩家在终点做一次同样速度的弹射，弹跳继承将玩家当前的下落速度，并使玩家向上弹射，这可以让玩家进行一些有想象力/有趣的关卡。你可以理解成V社游戏[《传送门》](https://store.steampowered.com/app/400/Portal/)系列那样的入门和出门机制。

3. 障碍物与倒计时开关门色块![BREAKABLE](images/BREAKABLE.png)![GENERICHOLD](images/GENERICHOLD.png)  
这两个色块通常用于阻碍/拖延玩家在关卡内的行进

- 障碍物色块![BREAKABLE](images/BREAKABLE.png)  
射击可摧毁的障碍物（高5个高度）被击中/损坏，直到其破坏（计算命中数，而不是实际伤害）  
障碍物耐久值(hits) = 5 + 障碍物耐久倍率*当前服务器玩家总数  
![BREAKABLEREF](images/reference_breakable.png)  
- 倒计时开关门色块![GENERICHOLD](images/GENERICHOLD.png)  
按 E 来触发这个门（高5个高度）。一旦触发后，它将X秒（X可能因某些情况而异，如当前主题等）后打开，和开关门类似。  
![GENERICHOLDREF](images/reference_generichold.png)  

如果想了解更多颜色代表的各种地块，请查阅Luff提供的[绘画工具](http://www.luffaren.com/misc/PixelPaint/pixel-paint-master/index.php)里面的文档说明。

### 5.6 简单总结

通过了解这些基本的色块，现在我们可以读出部分地图信息。以刚才的Turnabout关卡举例，我们可以读出很多的信息：  
![MINIMAPINFO](images/MINIMAPINFO.png)

## 6. 关卡主题

不同的主题会有不同的难度和外貌。体现在关卡装饰物、液体以及墙壁道路等方面。

- generic  
![generic](images/generic.jpg)
- castle  
![castle](images/castle.jpg)
- factory  
![factory](images/factory.jpg)
- temple  
![temple](images/temple.jpg)
- nature  
![nature](images/nature.jpg)
- hell  
![hell](images/hell.jpg)
- frost  
![frost](images/frost.jpg)
- silenthill  
表世界  
![silenthill1](images/silenthill1.jpg)  
里世界，此时人类触碰有害液体将会变成1hp  
![silenthill2](images/silenthill2.jpg)

Finale的主题是混乱的，它糅合了所有的主题。
无限关的主题会随关卡的进行而改变。

## 7. 地图事件

在 Finale 中只有贴门炸弹和人类低重力事件不会刷，其他事件均可发生。

### 7.1 事件刷新机制  

通常情况下地图事件只会在生成下一个关卡的时候产生。

一般事件由一个保底的基础概率（通常15%，具体事件刷新概率请查看 [3.2.1 关卡难度](#321-关卡难度) 一节。）和累加概率共同决定（通常是5%），如果一个关卡内没有刷事件，则会往概率上累加概率值。  
事件发生之后会有一个 事件CD ，这个 事件CD 值会在0~5之间随机生成，同时每通过一个关卡之后会让事件CD-1直至归零。

举个例子，比如玩家在stage 4，stage 4的事件刷新保底概率是30%，我在开头生成的第一个小关卡没有产生事件，则会往这个概率上面累加10%，从而在生成下一个关卡的时候会有40%的概率随机产生一个事件，事件也有其他因素影响比如关卡的性能开销等。然后如果在下一个关卡没有产生事件，还是继续往这个概率栈里面累加10%，这时再生成下一个关卡产生事件的概率将会变成50%，一直到有事件发生为止。事件发生后，会产生相应的事件CD（stage4为0~3个关卡），在这个事件CD内产生的关卡通常情况下都不会再产生新的事件，并且每通过一个关卡让这个事件CD-1直到其变为0。

### 7.2 事件列表  

- **PIZZA OF DOOM**  
![PIZZAOFDOOM](images/PIZZADOOM.png)  
披萨从天而降，开枪或被毁灭。
基本血量500，每个人类增加1000血。
- **PLEDGE**  
![PLEDGE](images/PLEDGE.png)  
我宣誓为collective尽一份力！  
`i pledge to do my part for the collective`  
在聊天框输入这段话即可。未宣誓者将每秒流失2hp直到去世。  
未宣誓者之死  
*`NyaaaDoge did not state the pledge`*  
- **KAMIKAZE**  
![BANZAI](images/BANZAI.png) ![BANZAI2](images/BANZAI2.png)  
将母体僵尸选为神风飞机的驾驶员以自爆的方式冲向人类，人类需要将其击坠或躲在掩体之后。初始血量250，每一个人类增加50血。
- **BEAMS**  
![BEAMGRID](images/BEAMS.png)  
天坠激光会从人类头上坠落。钻空隙躲避，碰到直接秒杀。
- **WORLD EATER**  
![WORLDEATER](images/WORLDEATERVAUFF.png)  
天上有一张大脸，射爆他，不然他就一直看着你。吞噬世界。如果没打掉，他会一直跟着人类  
大脸初始血量1000，每个人类加500血，每个僵尸加250血
- **THICK FOG**  
![THICKFOG](images/THICKFOG.png)  
人类的视野暂时受浓厚迷雾阻碍，持续40s。
- **BLOODLUST**  
渴血事件。人类很饥渴（每次掉2hp），需要射爆僵尸才能回血（每次射击僵尸回3hp），持续60s。
- **DEBRIS**  
![DEBRIS](images/DEBRIS.png)  
天上掉下各种地图方块的碎片，每块造成19hp，持续60s
- **LOW GRAV**  
人类获得20s的低重力，20s后直接切换成正常重力，人类要小心最后不要摔死了。
- **COLLAPSE**  
![COLLAPSE](images/COLLAPSE.gif)  
之前的关卡在逐渐分崩离析，该关卡内的所有的方块都会坍塌。
- **PHASING**  
![PHASING](images/PHASEING.png)  
人类的眼睛进行相位转移，参透世界，地图方块变得透明。持续20s  
*小心行事*
- **SILENCE**  
人类全体静音15s。15s逐渐消失，15s完全静音，10s恢复至正常。
- **WEAPON JAM**  
武器卡壳9s，期间会不停上子弹。
- **WALLBREAK**  
![WALLBREAK](images/NOWALLS.gif)  
触发事件时所有的墙壁格子会逐渐消失，不再恢复。
- **BIGNADES**  
![BIGNADES](images/BIGNADE.gif)  
人类手雷暂时获得增益40s，期间手雷变成大脸 ~~(和天降大脸一个模型VAUFF)~~ ，每颗雷对僵尸造成5000伤害，手雷伤害范围增大，也会有高击退效果。对Boss也能造成5000伤害，同时会有60%的几率眩晕Boss 5s。
- **DOORHUG BOMB**  
![DOORHUGBOMB](images/DOORHUGBOMB.png)  
*贴门炸弹，断后最爱，1点2秒，谁敢贴门？*  
通常只会在下张地图生成的时候产生该事件，左下角提示出现1.2s后爆炸，贴近伤害很高。通常情况下聪明的人贴门都会离终点光圈至少2格远以上，虽然还是会受到些许伤害，但不致命。
*断后部队不要怕，死的都是贴门的*
- **DISTORT**  
![DISTORT](images/DISTORT.png)  
人类全体获得扭曲视线，持续15s。  
*我瞎了*

## 8. 地图物品

大部分情况下物品都有使用次数和限制。详细请查看拾取后的说明。物品最多存在30个，如果超过该数量则新的关卡不会产生新的物品。  
如果关卡里面没有安排 人类/僵尸 物品生成点，则人类或僵尸物品会在关卡的起点色块![STARTENDTILE](images/START_END_TILE.png)刷新。

### 8.1 (未翻译)人类物品 HUMAN (TEAM 3)

- **dragonslayer(`0s`)**  
It was too big to be called a sword...  
Use it while falling to downslash  
Using it puts a strain on your body  
You cannot use it while too weak (`5hp`)  
Blood-buildup makes it heavier to wield  
WaterCrystal can wash the blood off  
FireCrystal can make it temporarily stronger  
- **baguette(`0s`)**  
Hold zombies back with wide swings  
The swings hurts+pushes zombies (and hurts itself)The baguette eventually breaks by too much damage  
(break-chance stacks by `0.10%` for each swing-hit)  
(break-chance stacks by `0.50%` for each swing-miss)  
A watercrystal can set the break-chance to `-15.00%`  
Can hurt/stun boss  
- **minislots(`1s`)**  
A portable slotmachine to gamble on-the-go  
Win chance: `5.00%`  
Lose: lose `7hp`  
Win: gain `42hp`  
- **billnye(`1x`)**  
Show nearby zombies a Bill Nye VHS  
Keep class distracted while you laze off  
Their attention gets drawn to the TV  
It lasts for `14s`  
Can stun boss  
- **peanutbutter(`5s|10x`)**  
Smear out a plane of peanut butter  
It slows zombies heavily for `6s` on-touch  
The smear lasts `15s`  
The same smear can't slow the same zombie twice  
The slowdown stacks  
Can hurt/stun boss on-spawn  
- **claymore(`10x`)**  
Plant claymores in front of you  
They blow up when zombies go in front  
They hurt, burn and stop zombies  
Can hurt/stun boss  
FireCrystal can stack-buff its damage  
- **piggyback(1 seat)**  
Allows a human to piggyback on you(they must press E on the saddle to get on/off)  
If you die/drop the knife, the player gets forced off  
The rider gets a jump/velocity-boost when getting off  
(allowing for a yoshi/boost-jump)Give someone a joyride!  
- **hackerman(`1x`)**  
Gain 10s of aim-hacking + infinite ammo  
Just keep firing and get kill after kill  
Nearby/targeted zombies become 1-hit  
Nearby zombies get wallhack-marked  
Can hurt/stun boss  
- **bhop_steroids(`30.00f`)**  
Inject yourself with steroids  
for automatic bunnyhopping!  
Limited/fuel-like usage  
Toggle it on/off with +use/E  
`2.00f` insta-drains on each activation  
You can clear a 4-tile gap from the edge  
- **planetcrystal(`1x`)**  
  1. EarthCrystal  
Spawns a wall just in front of you  
3 tiles wide, 2 tiles tall, stays up for `12s`  
Auto-breaks by certain human touches (anti-grief)  
Auto-breaks near main-teleport  
Can hurt/stun boss  
  2. FireCrystal  
Damage heavily + set zombies on fire for `10s`  
It also slows zombies slightly for `3s`  
The fire shoots out towards your front  
It also stops the zombie-velocity on-first-touch  
Can hurt/stun boss  
  3. WindCrystal  
Push zombies back with a single wind gust  
The wind shoots out towards your front  
It's active/stationary for `2s`  
Cancels z-gust projectiles  
Can hurt/stun boss  
  4. WaterCrystal  
Stop + slow zombies heavily for `10s`  
The water shoots out towards your front  
It deals no damage, only slowdown  
Can hurt/stun boss  
- **rift(`1x`)**  
Create a shortcut portal  
1st use: create entry portal (big)  
2nd use: create destination portal (small)  
Portal clears `100s` from 1st use / Z-touch  
Use it to help your defenders get back safely  
2nd use cannot be used over gaps  
- **storm blade(`150s`)**  
Freeze and weaken zombies with a dimension-breaking slice  
Z-hp gets reduced to `2%` of their current health  
It only freezes nearby zombies the first moment on-use  
Once the post-cut hp-cap hits, nearby z's gets slowed for `15s`  
Can hurt/stun boss  
- **heal orb(`1x`)**  
Places out a healing orb  
It heals `9hp` every `0.50s`(up to `150hp`)  
The orb lasts for `15s`  
The orb provides infinite ammo  
The orb provides +1 nade (once)  
通常情况下如果奶球不存在会在下一个关卡刷出来，即使用完了拿在身上也会判定为奶球存在  
- **moonboost(`1s`)**  
Gives an upwards boost  
Combine it with jumping for extra height  

特殊物品 卡丁车：  
kart(CONTROL BY MOUSE ONLY):  
Look upwards/center-height to accelerate  
Look downwards to slow down  
Look sideways to turn [relative to kart-rotation]  
Look straight down to get off[Locked for RACE ending]  

### 8.2 (未翻译)僵尸物品 ZOMBIE (TEAM 2)

- **squid(`1x`)**  
Throw a squid that inks on floor-impact  
It throws towards your look-direction  
It can also bounce on walls  
Blinds and slows nearby humans from the impact  
Inked humans (`10s`) can't use items  
- **pizzabaker(`10s|3x`)**  
Spawns a pizza-projectile in your look-direction  
It instakills humans on-touch  
It goes through walls  
- **fling(`1x`)**  
Flings humans away from you  
Push them off edges  
Or fling away their defenses  
- **bomb chuck(`10s|3x`)**  
Throw a bomb that blows up after `5s`  
It throws towards your look-direction  
Deals AOE/explosive damage  
- **roar(`1x`)**  
Push nearby zombies forward with a roar  
The push goes towards your side-look-direction  
Surprise the human defenses!  
It also heals you nearby zombies to `10000hp`  
- **greasy fingers(`1x`)**  
Makes nearby humans drop their held weapons(for `2 seconds`)  
You get one chance, use it wisely  
- **poise(`1x`)**  
Gives `1.50s` invincibility on-use  
Human items/bullets can't affect you  
Nearby humans also get frozen by fear briefly  
15x forward-moving illusion-copies spawn too  
Time it wisely, you only have one shot  
- **flight(`1x`)**  
Gives you wings to fly with until you die  
You get capped to `500hp`  
Humans you infect get TP'd back  
You TP back when too close to triggering current-stage end  
Fly by looking around and using WASD  
(you have slow momentum)  
- **gust(`10s|5x`)**  
Spawns a gust-projectile in your look-direction  
The gust pushes humans away  
It goes through walls  
- **puller(`10s|5x`)**  
Spawns a long, thin beam in your look-direction  
The beam pulls humans towards you  
It pulls after `2s`  
It deals `21dmg` on-pull  
- **stone(`3s|10x`)**  
Throw a stone that damages humans  
It throws towards your look-direction  
Deals `29 damage` on-hit  
- **impostor(`1x`)**  
Take human form for `15s`  
You teleport to a random human on-use(with `5s` invincibility)  
You cannot infect humans while in human form  
(humans can damage you though)  
Once your form reverts you can infect humans  
(infected humans get TP'd back)  
Your hp is dynamically capped until you die  
- **destructo hammer(`3s|5x`)**  
Break map tile(s) just in front of you  
(short radius, be accurate!)  
Destroys nearby human items  
Deals slight AoE-damage to humans  
Hit map tile(s) turn red and fall after `7s`  
Jumping through the broken tile-area slows Z's heavily for `10s`(slow-trigger disappears `7s` after the tile falls)  
Unusable during the early finale  
- **rift(`1x`)**  
Create a shortcut portal  
1st use: create destination portal (small)  
2nd use: create entry portal (big)  
Portal clears `100s` from 1st use  
Use it to help your zombie teammates ahead  
1st use cannot be used over gaps  
Entry becomes locked when too close to main-TP  

## 9. 陷阱地块

![TRAPS](images/TRAPSTILES.png)  
陷阱地块通常有三种类型  

1. Traps spawn
2. Traps vicinity
3. Traps step

### 9.1 Traps spawn

这个地块会生成以下陷阱

- **kart**  
![KART](images/KRAT.png)  
陷阱卡丁车，人类和僵尸都能进入。僵尸进入会触发圣战模式，碰到人就自爆。
操作方法(仅限鼠标操作)：
  - 向最头顶看可以跳跃
  - 向上看/高于中心高度加速
  - 向下看减速
  - 向侧面看转向[以自身卡丁车为中心旋转]
  - 向最底下看下车
- **thigh spider**  
![THIGHSPIDER](images/NPC.png)  
小腿腿NPC活蹦乱跳，粘在人类身上每咬一下造成3hp伤害
初始血量300，每个人类增加100血
- **button mimic**  
![buttonmimic](images/BUTTONMIMIC.png)  
红色的拟态按钮，谁按谁上当
- **explosive barrel**  
![explosive](images/EXPLOSIVE.png)  
炸药桶，射击1到30次之间会爆炸。
- **slot machine**  
老虎机，10%几率获胜获得150hp，每次输扣18hp。
使用次数在1到20次之间会爆炸，有40%的几率产生小老虎机神器。
- **mimic**  
![mimic](images/MIMIC.png)  
拟态神器，只要不去触碰就不会触发陷阱，碰到就原地去世  
*Tips: 你可以用 E-Pick 的方法检验神器的真伪，但是E-Pick仅限首次拾取神器有防 E-Pick 滥用机制，二手神器就没有这个保护机制了*  

### 9.2 Traps vicinity

这个地块会产生以下的范围型陷阱  
![TRAPSVICINITY](images/TRAPS.png)  

- **bomb**  
8秒倒计时的炸弹。*Back! get back!*
- **guster**  
效果和ZM风一样，会把人吹开
- **flinger**  
效果和ZM震荡一样，会把人震开
- **black hole**  
![BLACKHOLE](images/BLACKHOLE.png)  
生成一个黑洞，有强大的引力吸引人类，人类碰到其中心会去世，吸引一段时间后会消失

### 9.3 Traps step

这个地块会产生以下陷阱，只有玩家踩到该地块上才会触发

- **trap floor**  
![trapfloor](images/TRAPFLOOR.png)  
踩上去地板会消失，特征是地块上面有裂痕
- **landmine**  
![landmine](images/LANDMINE.png)  
*有地雷！小心脚下！*
- **bear trap**  
![beartrap](images/BEARTRAP.jpg)  
捕人器，人类踩上去-69hp顺带无法行动10s
- **pizza**  
![pizza](images/PIZZA.png)  
*THE PIZZA IS AGGRESSIVE*  
别管是什么陷阱了，不知道看不懂的东西别乱碰？？？不知道看不懂的东西别乱碰？？？不知道看不懂的东西别乱碰？？？
- **chatter curse**  
![curse](images/CHATTER_CURSE.png)  
地上会生成一个隐约可见的狮子头，人类踩一踩触发聊天扣字诅咒。每次损失2hp。
想解开诅咒需要在聊天框中输入屏幕显示的那段话。下面是所有可能的语句。
  - "i just farted really loud lol"
  - "wtf my teeth are so yellow"
  - "its not gay to take it up the ass"
  - "fuck my tight little hot pot pussy"
  - "my gf became pregnant yesterday"
  - "cant wait to suck off my bf later"
  - "ima ask mom to make me dino nuggies"
  - "subscribe to luffaren on patreon"
  - "my fingers are so fucking greasy"
  - "fucking poop ass balls tits fuck shit"
  - "ugh i feel so horny right now"
  - "my lips are meant for sucking"
  - "add me on steam for feet pics"
  - "my bf came in me last night what do i do"
  - "i always dreamt of becoming a cuck"
  - "googo gaga waah waah baby want milkies"
  - "i get really turned on by you"
  - "licking your own ass is hard af lol"
  - "i drink starbucks every single day"
  - "this map is the best map of all maps"
  - "my tits are starting to sag"
  - "my dick is actually really small tbh"
  - "my muscles are super big and cool i swear"
  - "guys steroids arent bad right"
  - "im high as fuck"
  - "i tried eating dog and its actually pretty good"
  - "brb my boyfriend is calling me"
  - "i think domestic violence should be legal"
  - "my ass is grass and i want u to smoke it"
  - "fuck i just realized i smell really bad atm"
  - "in full honesty cum doesnt actually taste that bad"
  - "let it be known that im gay"
  - "i wish that someone would peg me"
  - "i dare an admin to kick me"
  - "yo are any girls on the server rn"
  - "hey any girls here add me haha"
  - "fuck this ima pump my dick to xvideos"
  - "i wish this map had lasers"
  - "i deadlift 35kg im getting there"
  - "how do i get rid of itchy dick"
  - "giv eme your item plz"
  - "fuck my tight little zombie pussy"
  - "fuck yuor dont fall back bitchs"
  - "abcdefghijklmnopqrstuvwxyz"
  - "how do i use items"
  - "admin slay me you wont pussy"
  - "admin please slap me"
  - "do me harder oh yeah ah ooh"
  - "guys i cant hold it in anymore"
  - "i can lead this map better than you"
  - "anyone wanna play fortnite with me"
  - "im high as fuck"
  - "god i wish i could get laid"
  - "how do i get girl to touch my peepe"
  - "i pledge to do my part for the collective"
  - "i want luffaren to take my virginity"
  - "these zombie models make me horny"
  - "i did not cum on my cat"
- **spikes**  
![SPIKES](images/spike.png)  
各种游戏里面必不可少的经典款尖刺。
以150速度水平触碰会-23hp
以50速度垂直触碰会-132hp
- **banana**  
![banana](images/BANANA.png)  
可爱的香蕉皮，但是你踩上去自己转个五圈

## 10. 一些小彩蛋

你可能会在游玩地图的过程中看到这些Luff埋藏的小彩蛋

- 地图预定恶搞事件  
![MAPTROLL](images/MAPTROLL.png)  
你可能会看到左下角时不时出现 某某玩家预定/投票了某个地图 [1 vote]。
以下是可能会看到的地图列表  
  - ze_blackmesa_lambda_v1
  - ze_infiltration_final_p3
  - ze_predator_ultimate_p7
  - ze_toaster_p3
  - ze_halo_poa_p4
  - ze_interception_p2
  - ze_frostdrake_tower_v1
  - ze_castlevania_p1_7
  - ze_santassination_v3
  - ze_diddle_v3
  - ze_pizzatime_v9
  - ze_best_korea_v1
  - ze_magmadrake_b4
  - ze_eternal_grove_v3
  - ze_crazykart_v4
  - ze_collective_v1_9

- Steam/Discord 音效恶搞  
你可能会在游玩过程中听到自己Steam/Discord被敲打的音效，但是你跑出去看并没有被敲打！
最少需要5位玩家才能触发这个小彩蛋  
*只是一个音效播放恶作剧*

## 11. 写在最后

本指南只介绍了ze_collective中基本的组成部分。如果你想发挥你的想象力为ze_collective出一份力，去看看Luff给的绘画工具吧！笔者写这篇指南的动机是觉得ze_collective这张地图非常有意思，既可以在ze玩到肉鸽模式，也能用自己的想法简单实现一个关卡，甚至是快速实现部分小关卡的地图原型，难道不觉得很酷吗？这张地图的内核和玩法真的很有意思！即使刨除掉神器部分，其他的要素玩起来也是相当有意思！
