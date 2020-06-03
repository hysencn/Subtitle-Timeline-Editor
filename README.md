## 产品名：时间轴小助手
简单一句话介绍：这是个解决自己需求的个人作品    

### 当前状态：开发中
* 预计完成：2020年下半年（7月或8月）    

个人制作，无需汇报任何人，拖延症在所难免   

## 这款软件解决什么问题？
做字幕的时候舒服一些，高效一些

## 具体目标
1. 界面好看（也要有夜间模式）
2. 调整时间轴的效率高
	* 有快捷键
	* 背景有音频波形图，方便对齐

## 为什么做这个？
目前字幕编辑软件的体验很不好，   
因此做个新的，让做字幕的时候能舒服一些

## 软件设计图
![](./img/design.jpg)


## 幕后

### 其实做了很多个版本
![](./img/1.jpg)

### 缩放看到全景是这样的: 
![](./img/2.jpg)

## 分析
目前市面上可用来做字幕的软件有：   
* Aegisub
* Arctime Pro
* 人人译视界

它们的问题是

### Aegisub 的缺点
![](./img/aegisub.jpg)

* 2014年左右停止更新
* 界面不美观, 没有夜间模式，纯白界面看久了眼睛疼
* 快捷键的支持不够好，macOS 上不好用+容易崩溃
* 我从2013年用到现在2020年，忍够了

### Arctime Pro 的缺点
* 界面难看
* macOS 上用起来不舒服
* 时间轴一样的字幕块会叠加到一起，不方便做双语字幕

### 人人译视界的缺点
* 卡
* 难看
* 不好用

优点当然是功能很齐全，各种小工具都有，他们有很多用户      
用肯定能用，这是最基本的底线，    
我对这款软件的问题是用起来不舒服，不爽      

## 功能路线图

### 第一版
* 界面美观
* 调整时间轴方便
* 支持的格式有一个两个就行，不需要做太多兼容 (srt,ass,vtt)
* MVP 做出来就行
* 自用，可能暂不开源

### 第二版
* 做快捷键的设置和使用
* 其他待定   