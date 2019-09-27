# Douya
作者:
Zhang Hai

Douban, Inc.

Android Developer Intern

July 2016 – Sept. 2016, Beijing, China 
	
源代码：[https://github.com/DreaminginCodeZH/Douya](https://github.com/DreaminginCodeZH/Douya)	

***Material Design***

DrawerLayout

VectorDrawable

##### 笔记
系统5.0以上设置透明状态栏
> 
> view.setSystemUiVisibility(
                    View.SYSTEM_UI_FLAG_LAYOUT_STABLE | View.SYSTEM_UI_FLAG_LAYOUT_FULLSCREEN);
getWindow().setStatusBarColor(Color.TRANSPARENT)
[http://blog.csdn.net/guolin_blog/article/details/51763825](http://blog.csdn.net/guolin_blog/article/details/51763825)

允许使用transitions  
> getWindow().requestFeature(Window.FEATURE_CONTENT_TRANSITIONS); 

关闭shared element overlay
>setSharedElementsUseOverlay(false)

IntentService
>[鸿洋文章链接](http://blog.csdn.net/lmj623565791/article/details/47143563)

保存图片到系统
>[MediaStore.Images.Media.insertImage](http://blog.csdn.net/t12x3456/article/details/9099209)

StrictMode严苛模式
>[StrictMode就是用来指定一系列策略（policy），对相应规则（rule）进行检查并且做出反应。](https://www.jianshu.com/p/113b9c54b5d1)