# ✋[销售家](https://gitee.com/jianhuawan/XiaoShouJia.git)

#### 介绍
此项目不具备商业用途,仅供个人使用

#### 软件架构
- mvvm+retrfit2+rxjava架构
- fragmentation框架
- 数据库room
- 热修复tinker
- 加固(爱加密)
- 统计友盟
- 自动构建上传(jenkins+蒲公英)

####后续整合步骤

    - mvvm登录
    - 常规列表recycleView+详情跳转
    - 采用一个fragmentation架构 官方文档:
        https://github.com/YoKeyword/Fragmentation/wiki/2.-API
    - 网络请求用rxjava+retrofit2.0
    - weex整合
    - 热修复
    - 组件化(后续美团架构)https://tech.meituan.com/2018/12/20/modular-event.html
    - android 绘制流程https://www.jianshu.com/p/c151efe22d0d
    - android性能调优 jvm gc
    - 创建静态内部类的时候是不需要讲静态内部类的实例对象绑定到外部类的实例对象上。
      静态内部类属于外部类，而不是属于外部类的对象。
      只能访问外部类的静态成员变量或者静态方法。
      生成静态内部类对象的方式：Outer.Inner inner = new Outer.Inner()。
    - ConstraintLayout基本用法
    - android测试工具,算法知识,性能分析与优化
    - socket/tcp/ip/http/https
    - 内存优化管理,代码优化,第三方源码阅读或修改
    - 熟悉NDK
    - 熟悉rxjava,okhttp,retroit,databinding,lambaba,gradle脚本
    - 使用多线程,异步事件处理机制
    - git熟练,好处,分支和tag
    - 屏幕适配,多机型适配问题
    - 熟悉handler机制,自定义控件的绘制和事件分发机制
    - 熟悉java,熟悉虚拟机原理,数据结构和算法
    - android各个版本之间的差异,主要机型之间的差异
    - 熟悉android系统运行机制及内核,
    - 设计模式
    - room数据库,加密https://www.zetetic.net/sqlcipher/sqlcipher-for-android/
    - 集成友盟
    - gradle语法
    - okhttp原理
    - 组件化学习
    - 内存优化(精通)
    - kotlin
    - 深入学习GeekTime课程
    - 自定义图形图标(MPandroidChart)
    - 集成极光推送
    - 打包发布maven
    - 美团日志logan
    - markdown编辑个人简历
    - leakcanary内存检测,会造成系统anr
    - 利用breakPad抓取native异常
    - 常用算法和基本android技能汇总(pins工程模块化)

####问题集合

- fragment好处与低版本缺点,hide,show 和replace,fragment切换横屏怎么保存数据
- glide为什么会内存泄漏
- Arraylist和LinkedList
- 接口和抽象类



        jcenter注册地址:
        https://bintray.com/signup/oss  个人
        配置:
        https://blog.csdn.net/csdn576038874/article/details/79308391
        帐号:wanjianhua



        日志记录:
        https://github.com/Meituan-Dianping/Logan/blob/master/README-zh.md

        面试汇总:
        https://www.jianshu.com/p/20754b1adb4d



**1:handle消息机制**

message:又叫task,对消息进行封装,通过what来标识信息
Looper:循环者,通过perpre创建一个looper对象,Looper.loop轮询消息队列,是handle和message沟通的桥梁,一个looper只会被调用一次,保证消息不会串行
在ui线程做耗时操作会导致anr,通过handle将子线程的数据发送到主线程操作.

**19:屏幕适配,多机型适配问题**

老旧适配方案:

- 宽高限定符屏幕适配方案:在资源文件下创建不同分辨率的文件,
缺点:很多厂商机型宽高不确定
新方案:
- 今日头条屏幕适配方案通过反射适配系统的density值
- 限定符适配方案samllestwidth,这种方式是宽高限定符的升级版,只是把dimens.xml中的px换成了dp,
非常稳定，极低概率出现意外
不会有任何性能的损耗
适配范围可自由控制，不会影响其他三方库
在插件的配合下，学习成本低
但是替换成本高
- 鸿洋AndroidAutoLayout,停止维护
densit:密度=屏幕中1dp所占多少个像素点



    `markdown语法:
    https://guides.github.com/features/mastering-markdown/`
    
    `编译class为dex
    dx --dex --output=D:\dex\classes2.dex C:\Users\v-wanjh02\Desktop\dex`
    
    `androidx迁移,维护support,gradle3.3以上`







