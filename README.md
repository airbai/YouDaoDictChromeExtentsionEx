YouDaoDictChromeExtentsionEx
============================

#YouDaoDictChromeExtentsionEx 是在有道词典Chrome Extension的弹出框口上直接加一个“添加”按钮。用于将单词直接添加到单词本，不需要在有道词典页面去添加。

主要修改：
1. 在BackgroundPage.html增加“添加”按钮对应的html
2. 在lookup.js绑定“添加”按钮事件。点击按钮后多一次ajax GET请求到
http://dict.youdao.com/wordbook/ajax?action=addword&q=arduous&date=Thu%20Jun%2027%202013%2012:46:45%20GMT+0800%20(China%20Standard%20Time)&le=eng
如果当前Chrome有道帐户未登录则添加失败，自动弹出有道登录页面。


#原来UI：
![ScreenShot](https://raw.github.com/airbai/YouDaoDictChromeExtentsionEx/master/screenshots/original.png)

#修改后：
![ScreenShot](https://raw.github.com/airbai/YouDaoDictChromeExtentsionEx/master/screenshots/updated.png)
