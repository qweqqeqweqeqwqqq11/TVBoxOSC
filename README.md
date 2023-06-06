# TVBoxOSC
个人研究
1、修改软件名称地址

app/src/main/res/values/strings.xml

2、修改版本号地址

app/src/main/AndroidManifest.xml

3、修改图标、背景地址

你的地址/app/src/main/res

drawable/app_bg.png为背景，把原来的删掉，自己上传一个新的；

drawable-hdpi/app_icon.png为图标1，把原来的删掉，自己上传一个新的；

drawable-xhdpi/app_icon.png为图标2，把原来的删掉，自己上传一个新的；

drawable-xxhdpi/app_icon.png为图标3，把原来的删掉，自己上传一个新的；

drawable-xxxhdpi/app_icon.png为图标4，把原来的删掉，自己上传一个新的；

4、修改内置源地址

俊老仓库打开下面，第83行app/src/main/java/com/github/tvbox/osc/api/ApiConfig.java

takagen99大佬仓库

app/src/main/res/values-zh/strings.xml

5、修改默认缩略图、硬解、dns地址：app/src/main/java/com/github/tvbox/osc/base/App.java

添加以下代码

//自定义默认配置，硬解，安全dns，缩略图

       if (!Hawk.contains(HawkConfig.IJK_CODEC)) {            Hawk.put(HawkConfig.IJK_CODEC, "硬解码");        } 

       if (!Hawk.contains(HawkConfig.DOH_URL)) {            Hawk.put(HawkConfig.DOH_URL, 2);        }

       if (!Hawk.contains(HawkConfig.SEARCH_VIEW)) {            Hawk.put(HawkConfig.SEARCH_VIEW, 2);        } 
