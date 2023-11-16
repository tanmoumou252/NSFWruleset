## English
# [Sub2clash](https://github.com/nitezs/sub2clash) is a subscription conversion that can be run locally
The experiences of use is so cool, the VPN Service Providers for the clash with the common protocols are supported

Compiled for multiple platforms, including docker.

Indeed, recently there is a subconverter malicious injection led to the leak of subscription things

The injected link gets control of the entire machine, and the subscription is just a small incidental part of the process.

And I use local conversions largely for ease of use, not security.

A brief discussion of what is easy to use

1. the software will use the 8011 network port, with web-UI, you can directly fill in your multiple subscriptions, or multiple nodes
2. in v0.0.6 version, by inputting the old version of the long chain can be parsed out of the old version of the parameters already filled in.
3. you can use regular expression to streamline the node name.
4. adding *#Provider A* to the subscription link will prepend **Provider A** to the names of all the nodes of that service provider.
5. auto-generate country proxy-groups, use ***\- \<countries>*** or ***\- \<all>*** to indicate that you only need proxies for one country or you need them all..
6. you can use your own template to generate the final configuration
8. See [Original Repo](https://github.com/nitezs/sub2clash/blob/main/README.md#%E9%85%8D%E7%BD%AE) or [my sample](https://github.com/tanmoumou252/NSFWruleset/blob/main/sub2clash%E5%B8%A6rule-provider%E9%85%8D%E7%BD%AE%E6%A8%A1%E6%9D%BF.md) for more parameters.

> [!IMPORTANT]
> - Subscription links may have ***&flag=clash*** at the end to indicate that it is a clash subscription.
> - If it's not at the end of the link, then the final configuration you generate may only have one VPN provider's services.
> - If an individual node needs to appear under a specific proxy-group, write the node's location in the template ahead of generate.


## 中文
# [Sub2clash](https://github.com/nitezs/sub2clash)是一个可以在本地运行的订阅转换
使用体验很不错,机场给clash用的常用协议都支持了

编译了多平台,包括docker

确实最近有发生subconverter恶意注入导致泄露订阅的事情

那段注入的链接得到的是整个机器的控制权,订阅只是整个过程的一个小小的附带

而我使用本地转换在很大程度上是出于易用,而非为了安全着想

简单的讨论下易用在什么地方吧

1. 打开后占用localhost 8011端口,配有web-UI,可以直接填你的多个订阅,或者多个节点
2. 在v0.0.6版本里,通过输入旧版本的长链 能解析出旧版已经填入的参数
3. 可以使用正则表达式来精简节点名
4. 在订阅链接后加 *#机场A* 可以在该组所有节点前加上 **机场A**
5. 自动生成国家策略组,使用 ***\- \<countries>*** 或者 ***\- \<all>*** 表示只需要某个地区的和全都要
6. 可以使用自己编好的模板生成最终的配置
8. 更多参数查看[原项目](https://github.com/nitezs/sub2clash/blob/main/README.md#%E9%85%8D%E7%BD%AE)或[我的模板](https://github.com/tanmoumou252/NSFWruleset/blob/main/sub2clash%E5%B8%A6rule-provider%E9%85%8D%E7%BD%AE%E6%A8%A1%E6%9D%BF.md)

> [!IMPORTANT]
> - 订阅链接在末尾可能会加上 ***&flag=clash*** 来表示这是clash的订阅
>
> - 如果末尾没有它,那么你生成的最终配置可能只有单个机场
>
> - 单个节点要是需要出现在特定的策略组下,就在模板里提前写好该节点的位置

 

