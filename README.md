YouDaoDictChromeExtentsionEx
============================

#YouDaoDictChromeExtentsionEx 是在有道词典Chrome Extension的弹出框口上直接加一个“添加”按钮。用于将单词直接添加到单词本，不需要在有道词典页面去添加。

#主要修改：
1. 在BackgroundPage.html增加“添加”按钮对应的html
2. 在lookup.js绑定“添加”按钮事件。点击按钮后多一次ajax GET请求到
http://dict.youdao.com/wordbook/ajax?action=addword&q=arduous&date=Thu%20Jun%2027%202013%2012:46:45%20GMT+0800%20(China%20Standard%20Time)&le=eng
如果当前Chrome有道帐户未登录则添加失败，自动弹出有道登录页面。

#原来UI：
![ScreenShot](http://ww2.sinaimg.cn/large/61de38fejw1e62ujqd9f3j20eo07kaay.jpg)

#修改后：
![ScreenShot](http://ww1.sinaimg.cn/large/61de38fejw1e62ujtql1kj20ea07agmg.jpg)

#怎么用这个修改：
1. 安装[有道词典chrome划词插件](https://chrome.google.com/webstore/detail/%E6%9C%89%E9%81%93%E8%AF%8D%E5%85%B8chrome%E5%88%92%E8%AF%8D%E6%8F%92%E4%BB%B6/eopjamdnofihpioajgfdikhhbobonhbb)
2. 下载https://github.com/airbai/YouDaoDictChromeExtentsionEx/archive/master.zip ，解电脑上的插件文件。
文件位置：
Windows XP: 
%USERPROFILE%\Local Settings\Application Data\Google\Chrome\User Data\Default\Extensions\eopjamdnofihpioajgfdikhhbobonhbb\{版本号}\
Windows Vista/ Windows 7/ Windows 8: 
%LOCALAPPDATA%\Google\Chrome\User Data\Default\Extensions\eopjamdnofihpioajgfdikhhbobonhbb\{版本号}

