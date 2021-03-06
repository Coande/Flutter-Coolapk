# Coolapk Flutter

![Build Action](https://github.com/Cyenoch/Flutter-Coolapk/workflows/Build%20Action/badge.svg)

[Flutter Coolapk 官方网站](https://cyenoch.github.io/flutter-coolapk-website/)

## 兴趣使然

## 本项目主要适配桌面端（宽屏）

- 本项目使用 flutter master channel
- ~~由于 path_provider 目前没有足够好的 windows 实现，所有 ExtendedImage 对 windows,mac os 都关闭了 cache (找到了)~~
- 手机使用时(或是宽度小于高度)，导航功能移动至侧滑，而且体验并不是很好
- ~~窗口大小变更时会导致重新获取信息，请尽量避免 (解决了)~~

## 下载地址：（适合国内，但注意不要在这个网站上登录）

- 注意，版本的时间是错误的，要＋一天才是实际编译时间!!!
- <http://github-mirror.bugkiller.org/Cyenoch/Flutter-Coolapk/releases/>
- 根据你所用设备的版本进行下载
- 如果提示缺少什么什么dll，请安装这个 [VC_redist.x64](https://cyenoch.lanzous.com/ibkt3eh)
- 安卓版：（不懂就下载 armeabi-v7a 的）
  - app-armeabi-v7a-release.apk
  - app-arm64-v8a-release.apk
  - app-x86_64-release.apk

## 调试开发:

- Windows: flutter run -d windows

## 目录结构说明->

```emm
ios/ ios平台相关
android/ android平台相关
windows/ windows平台相关
linux/ linux平台相关
assets/ 资源文件夹
.github/workflows/ github Actions配置
lib/
  /network/
    /api/ 存放基本的api
    /model/ 存放常用的Model
  /page/
    /collection_list/ 与收藏有关的
    /detail/ 动态详情
    /image_box/ 显示图片的页面
    /auto_page/ 暂无
    /home/ 主页
    /launcher/ 启动页
    /login/ 登录页
    /product/ 数码详情页
  /store/ 全局状态
  /util/ 通用工具
  /widget/ 存放控件
    /data_list/ 数据列表控件(准备转成auto_page)
    /item_adapter/ item适配器
test/ 测试(基本不用)
```

## 功能完成情况

- [x] 登录
- [ ] 注册
- [ ] 首页
  - [x] 框架
  - [ ] 关注
  - [ ] 热榜
  - [x] 话题
  - [x] 酷图
  - [ ] 视频
  - [x] 问答
  - [ ] 看看号
  - [x] 直播
  - [ ] 酷品
- [ ] 数码
  - [x] 框架
  - [x] 排行榜
  - [ ] 手机
  - [ ] 数码
- [ ] item 适配
  - [x] emoji 显示
  - [x] 大部分 item 的显示
  - [ ] 大部分 item 的功能
- [ ] 各种子页面适配
  - [x] 数码详情页数据显示
    - [ ] 相关操作
  - [ ] and more....
- [ ] 动态详情页以及相关操作
  - [x] 动态内容
  - [x] 图文显示
  - [x] 点赞/取消点赞
  - [x] 点赞/取消点赞回复
  - [ ] 转发
  - [x] 回复消息
  - [x] 回复 别人回复的消息
  - [x] 回复 别人回复的消息 的消息
  - [ ] 评论排序
  - [x] 收藏/取消收藏
  - [ ] 举报
  - [ ] 举报回复
  - [x] 关注楼主
  - [x] 跳转到楼主/评论用户信息
  - [ ] 查看赞
  - [x] 查看评论
  - [x] 关注/取消关注楼主
- [x] 发动态
  - [x] 普通动态
    - [ ] ~~附带图片~~
  - [ ] ~~图文动态~~
- [ ] ~~发酷图~~
- [ ] 发二手
- [ ] 发图文
- [ ] 发提问
- [ ] 发话题
- [x] 搜索页
- [ ] 话题页
  - [ ] 关注话题
  - [ ] 话题页面对该话题进行发动态/图文/提问
  - [ ] 搜索此话题内容
- [ ] 酷图页
  - [x] 显示列表
  - [ ] 查看酷图
  - [ ] 保存酷图
  - [ ] 点赞/评论/转发/收藏
  - [ ] 举报
- [ ] 问答
  - [ ] 关注问题
  - [ ] 添加回答
  - [ ] 邀请回答
  - [ ] 转发提问
- [ ] 看看号相关
  - [ ] 订阅
  - [ ] 对某看看号进行发动态/图文/提问
- [ ] 直播
- [ ] 我(页)
  - [ ] 我的关注页
  - [ ] 我的收藏页
    - [ ] 新建收藏单
    - [ ] 分享/点赞/关注/修改信息/删除
    - [ ] 我的图文
  - [ ] 我关注的好友页
  - [ ] 关注我的好友页
  - [ ] 我的所有动态
- [ ] 用户信息页
  - [ ] ~~编辑资料~~
  - [x] 显示用户信息
  - [x] 显示动态/~~关注的应用~~/~~应用集~~/~~发现~~/~~评分~~/酷图/~~我开发的软件~~
  - [x] ~~分享~~/加关注/~~私信~~
- [ ] 通知页
  - [ ] @我的动态
  - [ ] @我的评论
  - [ ] 我收到的赞
  - [ ] 好友关注
  - [ ] 私信
  - [x] 显示通知
  - [ ] 清除通知

看起来还挺多的。。。

### 项目使用 Provider 进行全局状态管理,主要由两个全局状态,Theme 和 User

### item_adapter 目录下的 auto_item_adapter 进行 item 的适配

## 欢迎提交 pr

## 若果遇到了什么bug，或是有什么宝贵的意见，或是想找人一起打会游戏，

- 欢迎加入Flutter酷安，群聊号码：823690281

## 如果想加入到开发，或是学习Flutter欢迎进群 py 讨论

- [751659171](https://jq.qq.com/?_wv=1027&k=5iu6dt5)

### 欢迎给我点赞(star) 投币(捐赠) 转发(fork)三连支持=,=你的每亿点帮助都会转化成我的动力

<p align="center" hidden>
 <img src="https://ftp.bmp.ovh/imgs/2020/04/63315f1f7170f7b1.jpg" alt="Sample" emm="220 330" width="0" height="0">
	<img src="https://ftp.bmp.ovh/imgs/2020/04/2bbe6679a8505512.png" alt="Sample" emm="220 300" width="0" height="0">
</p>

## 以下是预览图(2020/3/2)

<https://i.loli.net/2020/03/02/D9ZJdzhjAqQ74XB.png>
<https://i.loli.net/2020/03/02/TSq5PFzanofbtGR.png>
<https://i.loli.net/2020/03/02/tYE1VaL3K4OxkXC.png>
<https://i.loli.net/2020/03/02/hTHY2XEmuLDqztS.png>
<https://i.loli.net/2020/03/02/JoIvknHV7muTAdC.png>
<https://i.loli.net/2020/03/02/8kLC3ySgwDroiMT.png>
