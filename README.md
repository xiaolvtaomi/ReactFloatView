# ReactFloatView
自定义悬浮窗--FloatView

2017年 3月28日，2.0版本ReactFloatView推出！

还在为悬浮窗的实现而发愁吗？还在为头疼的系统版本适应而发愁吗？请使用ReactFloatView！

ReactFloatView的优点：

1.各位开发者可以根据自己需求，在源代码基础上定制自己需要的悬浮窗；甚至可以直接运用在自己的项目代码中，所需要做得只是替换工程中的相关的美术素材。

2.完美适配4.0或者更高版本的android系统，当运行环境是6.0以上的系统时候，内置的权限模块将会发起权限申请。

3.2.0版本相对于1.0版本，使用上更加简单便利，权限模块、悬浮窗各个功能模块集成在ZSDK类中--（废弃了1.0版本直接继承ReactFloatViewActivity的做法，改为调用ZSDK类中各个方法实现）。

请各位开发者观看一下动态效果图：

![image](https://github.com/caozaolin/ReactFloatView/blob/master/xiaoguotu.gif)

ReactFloatView工程目录如下：

![image](https://github.com/caozaolin/ReactFloatView/blob/master/projectjieshao.png)

libary-reactfloatview：悬浮窗类库，里面包含了实现逻辑以及资源图片等等，自定义样式需要修改时候需要修改图中资源。

![image](https://github.com/caozaolin/ReactFloatView/blob/master/libraryjieshao.png)

ReactFloatView的可以划分为三个工作形态：

1.small形态，对应的逻辑均在FloatWindowSmallView类中：

![image](https://github.com/caozaolin/ReactFloatView/blob/master/FloatWindowSmallView.png)

2.big形态，对应逻辑均在FloatWindowBigView类中，每一个item都是一个view，可以在类中自行自定义item；

![image](https://github.com/caozaolin/ReactFloatView/blob/master/FloatWindowBigView.png)

3.brand形态，对应逻辑均在FloatWindowBrandView类中；

<img src='https://github.com/caozaolin/ReactFloatView/blob/master/FloatWindowBrandView.png'/>


app：一个悬浮窗展示demo

使用如下：首先在你的工程项目中，依赖libary-reactfloatview；

<img src='https://github.com/caozaolin/ReactFloatView/blob/master/shiyong2.png'/>

其次在主要activity中，在相关生命周期中，调用ZSDK类相关方法；

<img src='https://github.com/caozaolin/ReactFloatView/blob/master/shiyong3.png'/>

下一版本3.0更新预测，配合网络交互，通过网络返回json数据，显示相应的item，而非目前2.0版本写死4个item！

如若有问题，请联系我：

qq：649959008
qq群：246231638
邮箱：caozaolin@163.com
