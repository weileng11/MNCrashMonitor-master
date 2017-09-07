# CrashMonitor
Debug监听程序崩溃日志,直接页面展示崩溃日志列表，方便自己平时调试。
[![](https://jitpack.io/v/maning0303/MNCrashMonitor.svg)](https://jitpack.io/#maning0303/MNCrashMonitor)

## 截图

![](https://github.com/maning0303/CrashMonitor/raw/master/screenshots/crash_001.png)
![](https://github.com/maning0303/CrashMonitor/raw/master/screenshots/crash_002.png)
![](https://github.com/maning0303/CrashMonitor/raw/master/screenshots/crash_003.png)
![](https://github.com/maning0303/CrashMonitor/raw/master/screenshots/crash_004.png)
![](https://github.com/maning0303/CrashMonitor/raw/master/screenshots/crash_005.png)


## 如何添加
### Gradle添加：
#### 1.在Project的build.gradle中添加仓库地址

   ``` gradle
   	allprojects {
   		repositories {
   			...
   			maven { url "https://jitpack.io" }
   		}
   	}
   ```

#### 2.在app目录下的build.gradle中添加依赖
   ``` gradle
   	dependencies {
   	     compile 'com.github.maning0303:MNCrashMonitor:V1.0.2'
   	}
   ```

## 使用方法:
### 1:Application 的 onCreate()方法 初始化：

``` java

     /**
      * 初始化日志系统
      * context :    上下文
      * isDebug :    是不是Debug模式,true:崩溃后显示自定义崩溃页面 ;false:关闭应用,不跳转奔溃页面(默认)
      */
    MCrashMonitor.init(this, true);

```

### 2:文件的位置:
``` java

    /Android/data/包名/cache/crashLogs/

```


### 喜欢就Star一下吧!

### 注意:
当应用已启动就崩溃的无法打开页面,直接看通知或者去文件夹里面查看:/Android/data/包名/cache/crashLogs/

## 感谢:
#### 内部使用了一些三方库文件:
##### [StatusBarUtil](https://github.com/laobie/StatusBarUtil)
##### [NotifyUtil](https://github.com/wenmingvs/NotifyUtil)

## 推荐:
Name | Describe |
--- | --- |
[GankMM](https://github.com/maning0303/GankMM) | （Material Design & MVP & Retrofit + OKHttp & RecyclerView ...）Gank.io Android客户端：每天一张美女图片，一个视频短片，若干Android，iOS等程序干货，周一到周五每天更新，数据全部由 干货集中营 提供,持续更新。 |
[MNUpdateAPK](https://github.com/maning0303/MNUpdateAPK) | Android APK 版本更新的下载和安装,适配7.0,简单方便。 |
[MNImageBrowser](https://github.com/maning0303/MNImageBrowser) | 交互特效的图片浏览框架,微信向下滑动动态关闭 |
[MNCalendar](https://github.com/maning0303/MNCalendar) | 简单的日历控件练习，水平方向日历支持手势滑动切换，跳转月份；垂直方向日历选取区间范围。 |
[MClearEditText](https://github.com/maning0303/MClearEditText) | 带有删除功能的EditText |
[MNCrashMonitor](https://github.com/maning0303/MNCrashMonitor) | Debug监听程序崩溃日志,展示崩溃日志列表，方便自己平时调试。 |
[MNProgressHUD](https://github.com/maning0303/MNProgressHUD) | MNProgressHUD是对常用的自定义弹框封装,加载ProgressDialog,状态显示的StatusDialog和自定义Toast,支持背景颜色,圆角,边框和文字的自定义。 |
[MNXUtilsDB](https://github.com/maning0303/MNXUtilsDB) | xUtils3 数据库模块单独抽取出来，方便使用。 |
[MNVideoPlayer](https://github.com/maning0303/MNVideoPlayer) | SurfaceView + MediaPlayer 实现的视频播放器，支持横竖屏切换，手势快进快退、调节音量，亮度等。------代码简单，新手可以看一看。 |
[MNZXingCode](https://github.com/maning0303/MNZXingCode) | 快速集成二维码扫描和生成二维码 |
[MNChangeSkin](https://github.com/maning0303/MNChangeSkin) | Android夜间模式，通过Theme实现 |
[SwitcherView](https://github.com/maning0303/SwitcherView) | 垂直滚动的广告栏文字展示。 |
[MNPasswordEditText](https://github.com/maning0303/MNPasswordEditText) | 类似微信支付宝的密码输入框。 |
[MNSwipeToLoadDemo](https://github.com/maning0303/MNSwipeToLoadDemo) | 利用SwipeToLoadLayout实现的各种下拉刷新效果（饿了吗，京东，百度外卖，美团外卖，天猫下拉刷新等）。 |

