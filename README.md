## 产品名：时间轴小助手
[README in English](./README-in-English.md)

## 设计图 
![](./img/design.jpg)  
(使用 Sketch 设计)

## 当前状态：开发中
第一版预计完成时间：2020年下半年      

## 是个人还是公司作品？
个人, 开发出来解决自己的需求

## 解决什么问题？
做字幕时可以舒服一些，高效一些   

## 具体意思是：
1. 界面好看（也要有夜间模式）
2. 调整时间轴的效率高
	* 有快捷键
	* 背景有音频波形图，方便对齐

## 为什么做这个？
目前字幕编辑软件的体验很不好，   
因此做个新的，让做字幕的时候能舒服一些


## 设计的幕后

### 做了多个版本
![](./img/1.jpg)

### 缩放看全景是这样的: 
![](./img/2.jpg)

# 同类软件分析
可以做字幕的软件有：   
* Aegisub
* Arctime Pro
* 人人译视界

说明：这个列表当然不全，我忽略了不少小软件，  
那些软件一般只有 Windows 版，而且界面很难看（发布时间基本都是 2000年~2010年）

## Aegisub 的缺点
![](./img/aegisub.jpg)

* 2014年左右停止更新
* 界面不美观, 没有夜间模式，纯白界面看久了眼睛疼
* 快捷键的支持不够好，macOS 上不好用+容易崩溃
* 我从2013年用到现在2020年，忍够了

编程语言：根据开源代码，看起来是用 C/C++ 写的

## 感谢评论区内 [BingLingGroup](https://github.com/BingLingGroup) 在2020年8月18号 [对 Aegisub 的补充说明](https://github.com/1c7/Subtitle-Timeline-Editor/issues/4)，内容如下，粘贴过来方便其他人学习 Aegisub：
1. aegisub仍有人维护 https://github.com/wangqr/Aegisub ，关于字幕渲染的插件VSFilter仍然有人在更新 https://github.com/qwe7989199/aegisub_scripts/releases/tag/v1.3 ，开源压制界的软件Avisynth和Vapoursynth用的人还有很多
2. 界面可以改颜色 `偏好设置-界面-颜色` 或 `偏好设置-自动保存` 中的上级目录的 `config.json` 文件中修改
3. `偏好设置-热键`
5. Arctime的优点竟然是波形图？你知不知道Aegisub也有波形图？音频区从右到左第三个按键是什么？另外频谱图比波形图好用是公认的吧，你觉得频谱图不好看，可以去 `偏好设置-高级-音频-频谱模式-质量-极高质量` 调整即可
6. Aegisub有视频区域脱离，`菜单栏-视频-拆分视频`
7. Aegisub已经有视频压制插件 https://github.com/qwe7989199/aegisub_scripts
8. 机翻可以考虑subtitleedit，当然谷歌翻译质量不是很好。deepl目前还没有免费的api可以白嫖，我的方案是把英文字幕抽取出来手动复制到网页端deepl进行翻译，再复制回去

## Arctime Pro 的缺点
![](./img/arctime.jpg)

* 界面难看 (以我个人的审美标准)       
* macOS 上用起来不舒服       
  (左上角视频区域和其他部分感觉"不是一个整体"，拖动窗口以及切换到其他程序时，视频区域的行为不一致，拖动时这个区域似乎在努力跟随，切换时会覆盖到别的内容）
* 直接拖入 ass 字幕文件时，时间轴一样的字幕块会叠加到一起，不方便做双语字幕      
 （据说可以根据不同样式导入到不同轨道，这样就不会叠在一起了，我改天试试）
* 右上角的文字区域是用来粘贴文字和输入文字的，就是把完整的文字稿放那里，只需要打轴，这对创作者很好，但是对翻译者没啥用，关又关不掉。界面布局没法做修改，虽然也不是什么影响使用的大问题，但就是不爽

优点:  
* Arctime 有音频波形图

补充：
* 编程语言：根据官网说明是 Java 写的，不知道是 JavaFX 还是 Swing（也不重要了，反正就是烂）          
* 用户挺多的 (我加的 QQ 群是第7个群，这个群有2000人，假设前面6个群也是2000人，就是2000*7=一万4千人）    
不知道这些用户怎么想的，我反正用起来不爽，用户估计是没有替代方案才用 Arctime

## 人人译视界的缺点
![](./img/rr.jpg)

* 卡
* 难看

优点：
* 功能很齐全，各种小工具都有

他们有很多用户，软件用肯定能用，这是最基本的底线，       
但是用起来不爽，反正在我的 macOS 机器上 (Macbook Pro 2017 15寸 16G内存) 各种卡顿         

现在"假设"他们完全解决了性能问题。不卡了。很流畅。     
但这个界面外观和操作方式，对我个人来说还是不爽，    
毕竟做个字幕少说也要3小时到2天。整天盯着这个影响心情（当然也可以说是我"要求太高了"）      
他们的界面设计原则就是有啥功能就全部堆叠到界面上，一个一个摆，整个界面看起来很臃肿，不简洁。     

## 用户群体分析
做字幕的人，基本只有2种角色：
1. 翻译视频的人（字幕组/自己一个人的字幕组，字幕一般做成双语）
2. 原创者 （自己做了个视频，然后希望加字幕，多数情况下只需要单语字幕，比如视频里说的是中文，就加中文字幕）

说这个的意义是，因为本软件作者是第一类人，那么在软件的前几个版本，会偏向第一种使用场景。   
也就是说复制粘贴完整的文字稿，然后用快捷键一边播放一边把一句句话填入到时间轴里，这样非常方便原创者的功能，暂时不会做。
原创者也需要各种导出功能，方便导入到  Final Cut Pro 或者是 Adobe Premire 或者是其他软件里。   
多格式导出功能的优先级在一开始也不会那么高。会做，但是会排后一点

## 功能路线图
### 总体来说:
* Aegisub 大大小小的功能太多了，一时半会儿肯定替代不了 Aegisub，先不以这个为目标
* 先把调整时间轴，改字幕文本，增删字幕的整体操作做舒服了，其他的再说      

### 1.0 版
* 好看
* 流畅
* 调整时间轴方便
* 字幕文件的类型，支持一两个就行，先简单做做，不要把大量时间花在格式兼容 (srt,ass,vtt 里面选一个做)

### 1.5 版
* 快捷键 （包括设置和使用）

### 2.0 版
* 加入机器翻译功能（先支持百度和彩云小译，先这两家）
* 加入视频压制功能

### 2.5 版
* 对 ASS 格式的各种高级功能提供更好的支持，比如样式，位置，颜色

### 3.0 版
* 语音转文字功能（先支持阿里云）

### 3.5 版本
* 对竖屏视频（比如抖音/instagram) 提供更好的支持，比如左侧完全被竖屏视频占满，让高度占满整个可见屏幕

### 4.0 版本
* 视频区域支持脱离，比如 Final Cut Pro 可以把视频区域单独弄到一个屏幕上  
比如你有2个屏幕，一个笔记本+一个外接显示器，    
视频可以在另一个屏幕全屏


# 近期(2019年之后)出现的字幕编辑软件
* [Nosub](https://github.com/patui/Nosub): Nosub Subtitle Editor，支持 Windows, 暂不支持 macOS  
[软件截图，视频演示，以及相关讨论看这条 Github issue](https://github.com/1c7/Subtitle-Timeline-Editor/issues/4)
