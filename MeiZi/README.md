# MeiZi	
作者&设计:drakeet 数据来自代码家的干货网站：http://gank.io
	
源代码：[https://github.com/drakeet/Meizhi](https://github.com/drakeet/Meizhi)	
	
WebView常用配置	进度显示,网页标题显示在ToolBar

***Material Design*** 	*CoordinatorLayout+AppBarLayout+CollapsingToolBarLayout+ToolBar*

FloatingActionButton.Behavior	自定义Behavior

TextSwitcher	该View具有设置动画的API-setInAnimation,setOutAnimation(直接使用系统提供的淡入淡出)

RxJava 使用多种操作符	

Retrofit 解析时间指定一个固定的格式	GsonConverterFactory.create(gson) setDateFormat("yyyy-MM-dd'T'HH:mm:ss.SSS'Z'")

单个gradle文件统一管理所有module的共有编译信息	"compileSdkVersion buildToolsVersion minSdkVersion targetSdkVersion
versionCode versionName"

Gralde控制生成APK文件名称	

Retrolambda使用	

Otto 是square公司出的一个事件库（pub/sub模式），用来简化应用程序组件之间的通讯。

AlarmManager+BroadcastReceiver+HeadsupCompat(第三方Library) 定时弹出悬挂式Notification 看下图
![screenshot1](./images/screenshot1.png)

横竖屏切换布局的处理(当前版本在清单文件中使Activity强制竖屏,相关代码不执行了)

TextView设置2种不同样式文本

RecyclerView的Item布局中某个View执行显示动画，非整个Item的显示动画

##### 笔记
> ImageView显示的图片资源可以是通过XML属性或者Java代码指定显示的图片内容，可以通过设置Resource、Uri 、Bitmap对象、Drawable对象来指定。  
> 
> ScaleType属性的修改本质上根据设定的枚举将变换赋值给mMatrix，最终通过onDraw中的矩阵操作实现。
> 	
> ImageView 的scaleType 属性 [http://www.jianshu.com/p/32e335d5b842](http://www.jianshu.com/p/32e335d5b842)

> cropToPadding属性可以让图片内容是在padding基础上进行变换（缩放，移动），根据实践如果使用了mScrollX mScrollY属性或者scaleType设置为MATRIX类型时会配合用到这个属性

>adjustViewBounds属性主要是让ImageView根据图片原有比例的约束下将调整大小，注意必须要限定住宽或者高，即将其中一个属性设置为match_parent或者确定尺寸。
>
>ImageView学习笔记 [http://www.jianshu.com/p/1fa1321f106c](http://www.jianshu.com/p/1fa1321f106c)

-
> AppCompatTheme 包含背景点击效果 "?attr/selectableItemBackground" -视图范围内展示波纹效果
> ![image1](./images/image1.gif)
> 
> ?android:attr/selectableItemBackgroundBorderless –将波纹效果延伸至视图之外。
> 
> ![image1](./images/image2.gif)

- 
> Android5.0新特性推出了悬挂式Notification [http://www.jianshu.com/p/e766ce44268b](http://www.jianshu.com/p/e766ce44268b)

-
>Fragment

>setRetainInstance(true) 旋转时 Fragment 不需要重新创建。fragment始终持有父Activity的引用,即使在父Activity被销毁和重新创建之后。
>
>setHasOptionsMenu(true) 无论如何, 你必须在 onCreate() 期间调用 setHasOptionsMenu() 来指出fragment愿意添加item到选项菜单(否则, fragment将接收不到对 onCreateOptionsMenu()的调用)