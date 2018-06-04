# Web Wallet 操作手册

Web Wallet 是 Egretia 团队提供给开发者的网页端钱包。区块链游戏开发和传统游戏开发另一个非常大的区别在于，区块链游戏需要经常和区块链进行交互，所以会频繁的和钱包打交道。虽然市面上有 Metamask 等第三方钱包，但是对于 Egretia 工作流来说不是非常方便，所以 Egretia 团队开发了本地调试钱包 Web Wallet。

在区块链游戏的开发过程中，Web Wallet 是嵌入到游戏中的，这样调试游戏的时候就可以方便的使用。

## 钱包登陆

Web Wallet 登陆目前分两步，第一步需要使用 Egretia Server 的助记词，第二步需要使用密码登陆。

![](../egretiaserver/pic1.png)

打开 Egretia Server，获取助记词。

![](../egretiaserver/pic1.png)

然后使用 Wing 点击调试游戏，调出 Web Wallet 页面，点击**使用助记词导入钱包**

![](../egretiaserver/pic1.png)

然后输入助记词和密码，这个密码是以后用来登陆 Web Wallet 的密码。

![](../egretiaserver/pic1.png)

以后登陆只需要使用密码即可，当然开发者随时可以使用助记重新导入钱包。

## RPC 连接

在 Egretia Server 的**设置**里可以设置 Egretia Server RPC 服务器的地址，Web Wallet 就需要设置这个地址才可以正常使用。

![](../egretiaserver/pic1.png)

通过 Egretia Server 获取 RPC 地址。

![](../egretiaserver/pic1.png)

打开 Web Wallet RPC 设置页面，粘贴保存，即可获取 Egretia Server 数据。

![](../egretiaserver/pic1.png)

## 转账

钱包登陆成功后可以查看目前的余额和对应的美元，当然开发者可以进行转账，举例来说，开发者从地址`0x939493274924093`转账给`0x939493274924093` 10 ETH。

![](../egretiaserver/pic1.png)

点击转账，输入 10，点击提交，输入密码即可。

![](../egretiaserver/pic1.png)

## 支付

以上内容描述了 Web Wallet 的基础功能，而游戏如何和 Web Wallet 进行交互呢？以 AVG 示例为例。

![](../egretiaserver/pic1.png)

我们购买 0.5 个还魂丹，需要 1 个 ETH，点击按钮。

![](../egretiaserver/pic1.png)

弹出 Web Wallet 确认窗口，输入密码即可。

![](../egretiaserver/pic1.png)

