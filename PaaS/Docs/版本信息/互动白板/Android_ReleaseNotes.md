# Release Notes - Android
## 2.3.5.224 @ 2019.10.30
- 增加跳转白板页步数的回调接口(onTEBGotoStep)
- 增加获取指定文件的缩略图接口(getThumbnailImages)
- 修改白板缩放过程中会产生Crash的问题; 
- 修复白板放大后精度丢失各端画面不对齐的问题

## 2.3.4.192 @ 2019.09.25
- 涂鸦屏蔽多指触摸
- ppt点击事件透传
- 移动端ppt翻页交互支持左右滑动翻页

## 2.3.3.135 @ 2019.08.19
1. 白板
    - 支持大房间1000人以上、低延迟视频；

## 2.3.2.125 @ 2019.08.07
1. 白板
    - 直线工具支持虚线和箭头样式；
    - 椭圆工具支持按固定起始或圆心点进行绘制；
    - 增加addTranscodeFile接口,用于转码文件的显示；
    - 去掉设置字体的接口
    
## 2.3.1.118 @ 2019.08.01
1. 白板
    - 修复文本框选不精确问题；
    - 增加内置字体，保证各端文本输入功能采用字体一致；
    - 增加各个工具鼠标样式；
    - 激光笔交互优化；
    - 增加加载完历史数据前，禁止调用操作白板接口的保护逻辑；

## 2.3.0.109 @ 2019.07.18
1. 白板
    - 首屏渲染优化;
    - 支持画出白板再画入；
    - 增加ppt加载css,js失败重试逻辑

## 2.2.2.99 @ 2019.06.30
1. 白板
    - AddFile接口同步返回FileID;
    - onTEBFileUploadProgress回调接口返回FileID和进度百分比；
    - onTEBFileUploadStatus回调接口返回FileID和错误码

## 2.2.0 @ 2019.06.20
1. 白板
    - 支持白板上下页跳转是否重置步数
    - 支持获取指定文件id的文件信息
    - TEduBoardErrorCode增加错误码
    - TEDU_BOARD_ERROR_TIM_HISTORYDATA 同步历史数据失败
    - TEDU_BOARD_ERROR_RUNTIME 白板运行错误

## 2.1.0 @ 2019.05.29
1. 白板
    - 支持图片预加载功能；
    - 支持是否将涂鸭数据同步给其他端功能；
    - 优化涂鸭笔迹去锯齿，让线条变得更平滑；
    - 优化橡皮擦工具，支持滑动擦除;
    - 优化H5ppt错误提示，在H5ppt文件已经存在的情况下抛出警告;
    - 优化文档展示，支持独立设置白板宽高比，支持滑动缩放;；

## 2.0.0.2 @ 2019.05.22
1. 白板
    - 修改BUG；

## 2.0.0.1 @ 2019.05.15

1. 新增功能支持：
    - 白板
        - 新增使用网页作为白板的背景；
        - 新增工具鼠标的功能，可以方便的手势翻页；
2. 问题修复
    - 修正Demo中白板的构建方式，移到TIC SDK中统一初始和反初始化；

## 2.0.0_RC3 @ 2019.05.10

1. 新增功能支持：
    - 白板
        - 支持设置文本样式及字体属性
        - 初始化接口支持传入所有属性初始值
        - 初始化支持设置白板宽高比
        - `AddFile` 接口支持传入COS转码URL
2. 问题修复
    - Demo依赖的IM版本指定为4.3.81，修复最新版IM修改接口导致编译异常问题


## 2.0.0_RC2 @ 2019.05.08

1. 新增功能支持：
    - 白板
        - PPT动画展示
3. 新增服务：
    - PPT动画转码服务


## 2.0.0_RC1 @ 2019.04.26

1. 新增功能支持：
    - 音视频通信
        - 实时音视频通信
        - 屏幕分享/播片（可与摄像头画面并存）
    - 云通信
        - 消息
        - 群组
        - 关系链管理
    - 白板
        - 涂鸦（铅笔、橡皮、激光教鞭、直线、空心椭圆、空心矩形、实心椭圆、实心矩形、文本）
        - 背景色、背景图
        - 点选、框选、移动涂鸦、撤销、重做
        - 白板缩放、移动
        - 文件展示（静态：支持PPT、PDF、WORD、EXCEL）、多文件支持
