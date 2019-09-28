# BilibiliLiveTools

Bilibili直播工具。自动登录并获取推流地址，可以用于电脑、树莓派等设备无人值守直播。

#### 致谢
Bilibili登录API以及部分工具类从项目[BilibiliAfk](https://github.com/wwh1004/BilibiliAfk "BilibiliAfk") Fork而来。本项目也是在项目[BilibiliAfk](https://github.com/wwh1004/BilibiliAfk "BilibiliAfk")基础上开发。

#### 前提条件
在Bilibili通过了实名认证并拥有直播间。开启直播间方式很简单，实名认证完了启用直播间就行。

#### 项目说明
（1）Bilibili  
Bilibili Api，包括登陆、开启直播之类的操作都封装在里面，直接调用即可。  
（2）BilibiliLiveCategoryList  
直播分区获取获取工具，可以通过此工具获取直播分区。  
（3）BilibiliLiveTools  
一键开启直播工具。  
[![Demo](https://github.com/withsalt/BilibiliLiveTools/blob/master/doc/demo.jpg "Demo")](https://github.com/withsalt/BilibiliLiveTools/blob/master/doc/demo.jpg "Demo")

#### 如何使用
首先在Users.json配置Account（登录名称）、Password（密码）。如下所示：
```json
[
  {
    "Account": "xxxxxxx",
    "Password": "xxxxxxxxxxx"
  }
]
```

配置LiveSetting.json中的LiveCategory（直播分类）、LiveRoomName（直播间名称）。如下所示：
```json
{
  "LiveCategory": "28",
  "LiveRoomName": "直播间名称"
}

```
然后运行程序即可。

#### 直播分区
开播时需要将ID填写到LiveSetting.json中的LiveCategory中。

|  ID | 分类名称  | 分区名称  |
| :------------ | :------------ | :------------ |
 | 260 | lol云顶之弈 | 网游 |
 | 86 | 英雄联盟 | 网游 |
 | 80 | 绝地求生 | 网游 |
 | 89 | CS:GO | 网游 |
 | 87 | 守望先锋 | 网游 |
 | 84 | 300英雄 | 网游 |
 | 83 | 魔兽世界 | 网游 |
 | 92 | DOTA2 | 网游 |
 | 91 | 炉石传说 | 网游 |
 | 82 | 剑网3 | 网游 |
 | 102 | 最终幻想14 | 网游 |
 | 240 | APEX英雄 | 网游 |
 | 239 | 刀塔自走棋 | 网游 |
 | 78 | DNF | 网游 |
 | 88 | 穿越火线 | 网游 |
 | 196 | 无限法则 | 网游 |
 | 115 | 坦克世界 | 网游 |
 | 248 | 战舰世界 | 网游 |
 | 164 | 堡垒之夜 | 网游 |
 | 93 | 星际争霸2 | 网游 |
 | 181 | 魔兽争霸3 | 网游 |
 | 114 | 风暴英雄 | 网游 |
 | 249 | 星际战甲 | 网游 |
 | 251 | 枪神纪 | 网游 |
 | 81 | 三国杀 | 网游 |
 | 112 | 龙之谷 | 网游 |
 | 173 | 古剑奇谭OL | 网游 |
 | 166 | 逆水寒 | 网游 |
 | 176 | 幻想全明星 | 网游 |
 | 252 | 逃离塔科夫 | 网游 |
 | 107 | 其他游戏 | 网游 |
 | 35 | 王者荣耀 | 手游 |
 | 256 | 和平精英 | 手游 |
 | 163 | 第五人格 | 手游 |
 | 268 | 王牌战士 | 手游 |
 | 255 | 明日方舟 | 手游 |
 | 37 | Fate/GO | 手游 |
 | 40 | 崩坏3 | 手游 |
 | 269 | 猫和老鼠 | 手游 |
 | 262 | 重装战姬 | 手游 |
 | 140 | 决战！平安京 | 手游 |
 | 113 | 碧蓝航线 | 手游 |
 | 250 | 自走棋手游 | 手游 |
 | 154 | QQ飞车 | 手游 |
 | 156 | 影之诗 | 手游 |
 | 36 | 阴阳师 | 手游 |
 | 267 | 路人超能100 | 手游 |
 | 274 | 新游评测 | 手游 |
 | 258 | BanG Dream | 手游 |
 | 253 | 一起来捉妖 | 手游 |
 | 189 | 明日之后 | 手游 |
 | 50 | 部落冲突:皇室战争 | 手游 |
 | 141 | 荒野行动 | 手游 |
 | 39 | 少女前线 | 手游 |
 | 182 | 方舟指令 | 手游 |
 | 48 | 虚荣 | 手游 |
 | 41 | 狼人杀 | 手游 |
 | 42 | 解密游戏 | 手游 |
 | 184 | 神都夜行录 | 手游 |
 | 206 | 剑网3指尖江湖 | 手游 |
 | 203 | 忍者必须死3 | 手游 |
 | 178 | 梦幻模拟战 | 手游 |
 | 208 | 雀魂 | 手游 |
 | 186 | 球球大作战 | 手游 |
 | 212 | 非人学园 | 手游 |
 | 215 | 月圆之夜 | 手游 |
 | 238 | 约战:精灵再临 | 手游 |
 | 242 | 命运歌姬 | 手游 |
 | 214 | 雀姬 | 手游 |
 | 263 | 辐射：避难所Online | 手游 |
 | 264 | 苍蓝誓约 | 手游 |
 | 265 | 跑跑卡丁车 | 手游 |
 | 98 | 其他手游 | 手游 |
 | 236 | 主机游戏 | 单机 |
 | 217 | 怪物猎人:世界 | 单机 |
 | 273 | 无主之地3 | 单机 |
 | 216 | 我的世界 | 单机 |
 | 218 | 饥荒 | 单机 |
 | 272 | 一起开火车！ | 单机 |
 | 271 | 遗迹:灰烬重生 | 单机 |
 | 266 | 火焰纹章：风花雪月 | 单机 |
 | 245 | 只狼：影逝二度 | 单机 |
 | 261 | 马里奥制造2 | 单机 |
 | 257 | 全面战争:三国 | 单机 |
 | 244 | 鬼泣5 | 单机 |
 | 228 | 精灵宝可梦 | 单机 |
 | 237 | 怀旧游戏 | 单机 |
 | 254 | 往日不再 | 单机 |
 | 243 | 全境封锁2 | 单机 |
 | 221 | 战地5 | 单机 |
 | 219 | 以撒 | 单机 |
 | 270 | 人类一败涂地 | 单机 |
 | 241 | 圣歌 | 单机 |
 | 233 | 皇牌空战7 | 单机 |
 | 229 | 古剑奇谭三 | 单机 |
 | 232 | 了不起的修仙模拟器 | 单机 |
 | 227 | 刺客信条:奥德赛 | 单机 |
 | 247 | 探灵笔记 | 单机 |
 | 226 | 荒野大镖客2 | 单机 |
 | 230 | 任天堂明星大乱斗：特别版 | 单机 |
 | 220 | 辐射76 | 单机 |
 | 224 | 太吾绘卷 | 单机 |
 | 225 | 中国式家长 | 单机 |
 | 222 | 超级马里奥奥德赛 | 单机 |
 | 235 | 其他单机 | 单机 |
 | 21 | 视频唱见 | 娱乐 |
 | 207 | 舞见 | 娱乐 |
 | 145 | 视频聊天 | 娱乐 |
 | 143 | 才艺 | 娱乐 |
 | 199 | 虚拟主播 | 娱乐 |
 | 136 | 美食 | 娱乐 |
 | 123 | 户外 | 娱乐 |
 | 25 | 手工 | 娱乐 |
 | 28 | 萌宠 | 娱乐 |
 | 27 | 学习 | 娱乐 |
 | 33 | 映评馆 | 娱乐 |
 | 34 | 音乐台 | 娱乐 |
 | 190 | 唱见电台 | 电台 |
 | 192 | 聊天电台 | 电台 |
 | 193 | 声优 | 电台 |
 | 94 | 同人绘画 | 绘画 |
 | 51 | 原创绘画 | 绘画 |
 | 95 | 临摹绘画 | 绘画 |
 | 96 | 其他绘画 | 绘画 |
