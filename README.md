# TingPowerPoint 官方首页

> 陈希章 于 2019年3月

## 项目概述

这个是我发起的一个在Office 365客户端和现有服务中进行人工智能应用创新项目的一部分。这是一个基于VSTO技术开发的PowerPoint插件，希望能为PowerPoint带来语音方面的体验。这个想法有几个出发点

1. 为文档增加语音后，可以使得收到你的PPT的用户不仅仅可以看，也可以听，就好像你在现场跟他讲述一样。
1. 为视力不好的用户提供帮助，他们可以听文档的内容。
1. 通过自然语言技术，为你的文档提供更加易于被聆听的声音，而且不是让人倦怠的纯机器声音。
1. 可以批量生成语音文档。
1. 可以实现自定义语音，例如把你的声音合成进去，但是又不需要你亲自朗读。

这只是一个开始，精彩还会有更多，如果有大家的参与的话。

## 申请试用

欢迎大家加入早期试用机会，你的建议和反馈，可以帮助我改进这个插件设计，甚至有可能会真的出现在以后版本的Office 365中呢。还等什么，请通过 <https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR9NNufPMIKNJmM6xKHZY6M9UNzJZUzU1UEJYUEEzVFRLUU5EWUNEVUJBUy4u> 给我提交一些信息吧，你将会被加入到一个种子用户列表中，并且可以直接通过邮件和我取得联系。

## 如何安装

1. 你需要首先安装一个证书，请通过右键点击 [证书](/resources/aioffice.cer) ，然后选择“链接另存为”，请参考如下的安装步骤：

    ![第一页](images/2019-03-21-09-16-08.png)

    点击“安装证书”按钮

    ![第二页](images/2019-03-21-09-17-05.png)

    选择“本地计算机”，然后点击“下一步”

    ![第三页](images/2019-03-21-09-18-35.png)

    选择“将所有的证书都放在下列存储”，然后点击“浏览”按钮，然后选择“受信任的根证书颁发机构”，然后点击“确定”按钮，回到证书导入向导后，点击“下一步”按钮

    ![第四页](images/2019-03-21-09-21-24.png)

    点击“完成”按钮

1. 你可以点击 [安装程序](/resources/installer.exe)，选择“download”，然后在本地完成插件的安装。请注意，一定要用这种方式，之前发现如果点右键，选择“链接另存为”的话，下载的安装程序是不全的。

    ![下载应用](images/2019-03-21-13-47-20.png)

    > 如果你在安装过程中遇到问题，麻烦在<https://github.com/chenxizhang/tingpowerpointaddin/issues> 给我提交问题，你也可以给我发邮件（aioffice@xizhang.com）, 但无论哪种方式，请务必提供一下错误截图，以及你当前使用的Windows系统版本，PowerPoint版本，是否使用Office 365等信息。我会第一时间回复。目前我们测试过的是在Windows 10上面，使用Office 365自带的PowerPoint版本，其安装过程大致为1分钟，非常顺畅。

## 如何试用

成功安装后，请立即打开你的PowerPoint客户端，你将看到一些新的工具栏出现在“加载项”这个选项卡中。（英文版本是Add-ins)

![插件界面](images/2019-03-21-09-29-37.png)

当前版本，最核心的一个功能就是“根据备注生成语音”，它的做法是循环每一页幻灯片，只要你提供了备注文字的，就会把这段文字通过人工智能自然语音转化成一段声音（当前是女声），然后将这段声音插入到当前的幻灯片中。

![生成语音](images/2019-03-21-09-32-56.png)

在生成过程中，如果没有备注文字，会自动跳过。如果当前幻灯片已经有语音或者视频，也会自动跳过。

你现在就可以按F5键播放这个带有声音的PPT了，请注意，为了避免太过于突兀，你需要点击鼠标收听语音。（未来我可能会做成自动播放，或者让用户可以选择是否要自动播放）。

马上开始神奇的语音PPT之旅吧。

## 如何更新

这个插件使用了自动更新技术，你每次打开PowerPoint时它就会自动检测服务器端是否有最新版本，然后帮助你完成更新。

### [2019-3-31] 版本 1.0.14

1. 这个版本的声音会自动播放。
1. 增加了一个可以快速分享材料的功能。目前仅支持一天内的分享，到期会自动删除文件。你可以通过二维码方式分享你的文件。

![二维码分享](images/2019-03-31-17-01-08.png)

点击这个按钮，会做一些必要的检查

![分享确认](images/2019-03-31-17-02-20.png)

然后有一个窗口用来生成二维码

![二维码](images/2019-03-31-17-09-39.png)

## 如何卸载

虽然我不愿意看到这样，但如果你不想继续使用这个插件，你可以在“应用和功能”这个页面中，搜索TingPowerPoint，然后删除即可。

![卸载](images/2019-03-22-09-25-00.png)

## 隐私声明

为了帮助我们改进产品设计，该插件会收集一些匿名的数据，包括点击菜单按钮的顺序，以及当前PowerPoint的版本信息。这些数据不包含任何跟你个人有关的信息。

另外，因为需要用到在云端的人工智能服务，所以你在幻灯片的备注区域的文字会被发送到Azure认知服务API层，在插件层不会做任何保存。

## 欢迎推荐

如果你用的还不错，非常希望你能推荐给周围的朋友试用， 请通过 <https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR9NNufPMIKNJmM6xKHZY6M9UMVRRUVBBSkhMTEM0ME5BT0lLRUQwU01QVC4u> 填写相关信息，我会发送邮件给你的朋友，帮助他试用。

## 欢迎反馈

我非常希望得到大家的反馈意见，请通过 <https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR9NNufPMIKNJmM6xKHZY6M9UODlKWUg0MkJLQTlGSFdGU05KUjAzQURVNS4u> 这里提交你的意见和建议，谢谢！

