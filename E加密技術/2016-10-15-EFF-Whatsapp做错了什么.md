---
date: 2016-10-15
---

## 「譯」EFF：Whatsapp的四點不安全做法

譯者：MDrights

[原文鏈接](https://www.eff.org/deeplinks/2016/10/where-whatsapp-went-wrong-effs-four-biggest-security-concerns)（注：译者只进行了概括性翻译，请以原文为准）

作者：Gennie Gebhart

经过深思熟虑，我们（EFF）决定把对即时通讯软件Whatsapp的安全使用警示/注意事项，添加到我们的[自我防监控指导手册](https://ssd.eff.org/en)。

（译者注：EFF介绍了哪几点Whatsapp的不安全的地方呢？下面跳过原文的一些背景介绍，把这几个关键点翻译，供参考：）

- 备份是不加密的  
Whatsapp提供了把会话信息备份到云端的机制。为了在以后把这些信息可以从云端不需要密码恢复过来，这些备份必须是非加密的。在第一次安装的时候，Whatsapp会弹出提示让你选择多久备份一次：每天、每周、每月还是永不。在我们的《自我防监控指南》里，我们建议选择永不备份你的对话记录。同时为了确保你的信息得到加密，你的通讯对象的whatsapp也需要设置成永不备份到云端。

- 密钥变动的提醒  
如果你的通讯对象的加密密钥变换了，一个安全的通讯软件应该通知你并提示你选择是否接受。然而在Whatsapp，这并不是默认的设置。要想得到这个提醒，你需要到“设置”——“帐号”——“安全”——“安全提醒”，然后手动把它打开。密钥的验证很关键，用于预防一种叫作“[中间人](https://ssd.eff.org/en/glossary/man-middle-attack)”的攻击，即第三方可以假扮你与之通讯的对方和你通讯。如果你的通讯对象突然变换了密钥，有这几种原因：
1. 对方在别的手机上登录自己的帐号，或重装了whatsapp软件；
2. 中间人在别的设备上登录了对方的帐号，或截获了你与对方的通讯流量并进行了修改，然后与你通讯。
（此处译者略做细化；补充：如果出现这个密钥变更提示，建议最好与对方面对面密钥里的“指纹”是否一致，也即通过它那个二维码扫一扫便知，或肉眼核对。）

- Web版应用  
Whatsapp提供了基于HTTPS（有一定安全功能的）web（网页形式）用户界面。就跟其他所有使用了HTTPS的网站一样，即使用了TLS的流量加密，仍有很多可能让用户[登录到了一个仿冒的恶意的网站](https://www.wired.com/2007/11/encrypted-e-mai/)。（比如在访问HTTPS网站的初始请求有可能仍是http协议；以及关于HTTS网站CA证书问题，etc——译者）。那么一个更好的更安全的建议是应该开发个不使用web协议和界面的客户端作为手机端的拓展。

- 与Facebook的数据共享  
Whatsapp前段时间更新了其隐私政策，包括其将与母公司“非死不可”共享用户的信息以便推送广告。然而这份隐私政策并没有清楚地讲明用户的哪些信息会/不会被共享给FB。而且尽管它让现有用户可以选择不让Whatsapp把信息共享给FB中的“用户体验”部分，但用户无法选择不把信息共享给FB自己。因此FB仍是可以肆无忌惮地看到用户的通讯活动。

**建议**

Whatsapp和FB只要做到以下几点，就能赢回我们对该产品的信心：
1. 简化用户界面，一些安全选项设为默认，如关闭备份、开启密钥变换提醒、关闭信息共享等等。
2. 公开且具体得公告，它将与FB共享哪些用户数据，打算如何使用这些数据；还应说明它将对所收集的用户信息做什么，以及更重要的，是不做什么。


