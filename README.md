# ImagePicker
Android自定义相册，完全仿微信UI，实现了拍照、图片选择（单选/多选）、 裁剪 、旋转、等功能。

### 由于个人时间有限，该项目停止维护
如果你发现有bug，或者好的建议，可以提merge request，我测试通过后会立即合并并发布新版本，确保该库处于可用的状态。

该项目引用了：

* [(https://github.com/jeasonlzy/ImagePicker]((https://github.com/jeasonlzy/ImagePicker)

喜欢原作的可以去使用。同时欢迎大家下载体验本项目，如果使用过程中遇到什么问题，欢迎反馈。


## 1.用法

使用前，对于Android Studio的用户，可以选择添加:
```java
	compile 'com.lzy.widget:imagepicker:0.6.1'  //指定版本
```

## 2.功能和参数含义

### 温馨提示:目前库中的预览界面有个原图的复选框,暂时只做了UI,还没有做压缩的逻辑

|配置参数|参数含义|
|:--:|--|
|multiMode|图片选着模式，单选/多选|
|selectLimit|多选限制数量，默认为9|
|showCamera|选择照片时是否显示拍照按钮|
|crop|是否允许裁剪（单选有效）|
|style|有裁剪时，裁剪框是矩形还是圆形|
|focusWidth|矩形裁剪框宽度（圆形自动取宽高最小值）|
|focusHeight|矩形裁剪框高度（圆形自动取宽高最小值）|
|outPutX|裁剪后需要保存的图片宽度|
|outPutY|裁剪后需要保存的图片高度|
|isSaveRectangle|裁剪后的图片是按矩形区域保存还是裁剪框的形状，例如圆形裁剪的时候，该参数给true，那么保存的图片是矩形区域，如果该参数给fale，保存的图片是圆形区域|
|imageLoader|需要使用的图片加载器，自需要实现ImageLoader接口即可|
|hideImageFolders|隐藏的图片文件夹|

