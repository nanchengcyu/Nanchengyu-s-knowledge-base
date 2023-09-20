大家好，我是南城余！
终于不负众望，不再当鸽王。域名在经历了半个月终于备案成功了。
今天这篇文章它终于来了！
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1695199100151-b4c5bc1c-4806-4d4e-8d52-d71661e14cf1.png#averageHue=%23faf6f5&clientId=ue523ea05-ddde-4&from=paste&height=354&id=uf48e7e38&originHeight=442&originWidth=1026&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=39940&status=done&style=none&taskId=u9eed8a68-e66f-4e84-b561-b57a4794bf2&title=&width=820.8)
今天带领大家认识下域名。
全篇属于自己之前学到的一些知识，之前没做笔记，所以今天还是总结下，所以这篇文章高度属于我的纯原创内容。
**这绝对是全网第一篇带领你从学习到认识域名的好文，建议所有想学习域名，了解域名的人观看。**

今天的主要内容有
1.域名的认识
2.域名的实操（将自己的网站（服务器IP地址）与域名绑定）
3.以及域名走https协议实操

域名，是拜访你的网站的门户，下面我将用一文给大家讲解下，域名的知识，还有如何将你的网站使用的协议从http变为https
下面操作全部基于阿里云。其他平台类似。

一个域名其实大有学问的，你可以了解到这些知识
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1694881472117-93ac2983-f4d5-4bd2-aebc-a63ba72e7c34.png#averageHue=%23eef0f5&clientId=uf20e1123-4f70-4&from=paste&height=421&id=udcb21c08&originHeight=474&originWidth=1259&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=122504&status=done&style=none&taskId=uff191648-d964-4a89-9e95-8d5f760ad82&title=&width=1119.111111111111)
# 域名认识
### 域名基本知识
了解域名先从域名的基本知识开始，而链接域名的基本知识从了解域名的组成开始，可以看下下面的图片哦~
![](https://cdn.nlark.com/yuque/0/2023/jpeg/38420467/1694881804017-738a0955-10f7-4d99-ba36-2e54b47e6743.jpeg#averageHue=%23fdfdfd&clientId=uf20e1123-4f70-4&from=paste&id=u3e35f7fe&originHeight=687&originWidth=1300&originalType=url&ratio=1.125&rotation=0&showTitle=false&status=done&style=none&taskId=ud7c3aaa2-d378-4740-a6c0-bed4acdfc83&title=)
所以一般域名组成都是由四个组成部分构成，分别是顶级域名、二级域名、主机名和协议名。
域名的理解方法，与人类的直觉认识不同，理解一个域名要从右到左哦！
下面我拿百度的网址来给大家做个分析哦
> [https://www.baidu.com/](https://www.baidu.com/)

这是一个完整的域名
### 域名协议
前面http使网站使用的协议，一般协议分为http和https（有关这个协议，这是计算机网络的知识，大家可以看下我写的这篇推文[https://mp.weixin.qq.com/s/csnMjdI1NYtCzFEgSQp7xw](https://mp.weixin.qq.com/s/csnMjdI1NYtCzFEgSQp7xw)）
### 域名前缀
www:这个是自定义的，可以感觉自己的心情自己定义，一般选用www的原因，请看下面解析
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1694879447571-9b9a2da3-b321-43ee-b5c4-a19fe4998085.png#averageHue=%23edeff5&clientId=uf20e1123-4f70-4&from=paste&height=217&id=u3ec9946c&originHeight=244&originWidth=1190&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=69295&status=done&style=none&taskId=ud29c4737-be99-4776-bfee-099992abe48&title=&width=1057.7777777777778)
比如我买了个我自己的域名（nanchengyu.cn），然后我有多个网站，我想要做区分我就会选择在前面做区分
假设我创建了我的博客（myblog），然后还创建了一个BI数据分析平台(techmindwave)
这个时候我就可以将我的域名变为
我的博客（myblog.nanchengyu.cn）
BI数据分析平台(techmindwave.nanchengyu.cn)
### 域名后缀
域名后缀就是com,我选择的是cn,所以我的域名就是(nanchengyu.cn),和百度的不一样
#### 常见的域名后缀分类
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1694879969648-da6767d4-0433-44f6-9b46-97604a4a7bd9.png#averageHue=%23f0f1f6&clientId=uf20e1123-4f70-4&from=paste&height=498&id=uf27038f5&originHeight=560&originWidth=1114&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=125147&status=done&style=none&taskId=u627e6996-302b-4282-be12-fde31855489&title=&width=990.2222222222222)
所以你见到的我的后缀（cn）代表的就是中国的意思
#### 常见国家域名后缀分类
![](https://cdn.nlark.com/yuque/0/2023/jpeg/38420467/1694881663592-34b121d1-fd74-4146-a6e4-8dc55476da4d.jpeg#averageHue=%23706140&clientId=uf20e1123-4f70-4&from=paste&height=234&id=ubc484fc9&originHeight=234&originWidth=409&originalType=url&ratio=1.125&rotation=0&showTitle=false&status=done&style=none&taskId=u8b1ccf12-7eb0-4456-b9eb-d865e794b0f&title=&width=409)
#### 域名后缀的特殊情况
不知道你们看没看见过这种情况（.com.cn/或者.com/au）
下面给大家做个实例，拿苹果的网站给你们展示啊，这是国际大厂一般都会采用的区分不同国家地区的方法，你仔细观察身边你拜访过的网站应该都会有的，可以尝试下小米的，华为的等。
感兴趣的可以点击下方链接拜访下，看看哦！
[https://www.apple.com.cn/](https://www.apple.com.cn/)
这是苹果的大陆网站域名
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1694880478067-d96a3e91-d271-4147-8c4e-b4209c8dbfb2.png#averageHue=%233b3833&clientId=uf20e1123-4f70-4&from=paste&height=896&id=uadd3dd3a&originHeight=1008&originWidth=1911&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=346928&status=done&style=none&taskId=u3aaf8cfd-c4ff-4f1e-8cd0-ef2f3f2a829&title=&width=1698.6666666666667)
[https://www.apple.com/au/](https://www.apple.com/au/)
这是苹果的澳大利亚域名![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1694881061155-52453fb9-37f6-46e7-bf95-f1b30126a6f2.png#averageHue=%233b3833&clientId=uf20e1123-4f70-4&from=paste&height=847&id=u12b34988&originHeight=953&originWidth=1885&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=392998&status=done&style=none&taskId=u62f179cc-8724-4183-8f44-61ca6857e20&title=&width=1675.5555555555557)
大概大家都访问不了~哈哈哈，没事大家知道就行了
大家可以试试小米，华为的感受下哦~
我这里就不做演示了
还是贴一个链接大家试试吧
[https://www.huawei.com/cn/](https://www.huawei.com/cn/)
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1694881326432-3a03fcd8-9a05-4703-aed6-8c59c6f5c54b.png#averageHue=%23e9e9e9&clientId=uf20e1123-4f70-4&from=paste&height=892&id=ue2d767e7&originHeight=1003&originWidth=1920&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=461145&status=done&style=none&taskId=u99717b35-71fa-4578-8ebb-829b967dd53&title=&width=1706.6666666666667)
[https://www.huawei.com/au/](https://www.huawei.com/au/)
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1694881303319-ab212c16-2c5f-465a-b1f7-2e9112209d05.png#averageHue=%234f6634&clientId=uf20e1123-4f70-4&from=paste&height=823&id=ud205e196&originHeight=926&originWidth=1908&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=2292751&status=done&style=none&taskId=u55e31cf1-1d1d-4abd-88f8-85d23dafc07&title=&width=1696)


## 域名购买
[https://blog.csdn.net/pang_ping/article/details/101279960#](https://blog.csdn.net/pang_ping/article/details/101279960#:~:text=%E4%B8%80%E3%80%81%E5%A6%82%E6%9E%9C%E8%B4%AD%E4%B9%B0%E9%98%BF%E9%87%8C%E4%BA%91%E5%9F%9F%E5%90%8D%201%E3%80%81%E7%82%B9%E5%87%BB%E4%BA%A7%E5%93%81%EF%BC%8C%E6%89%BE%E5%88%B0%E5%9F%9F%E5%90%8D%E6%B3%A8%E5%86%8C%EF%BC%8C%E7%82%B9%E5%87%BB%E8%BF%9B%E5%8E%BB%E3%80%82,2%E3%80%81%E8%BE%93%E5%85%A5%E6%83%B3%E8%A6%81%E8%B4%AD%E4%B9%B0%E7%9A%84%E5%9F%9F%E5%90%8D%EF%BC%8C%E7%82%B9%E5%87%BB%E6%9F%A5%E8%AF%A2%E3%80%82%203%E3%80%81%E9%80%89%E4%B8%AD%E6%83%B3%E8%A6%81%E8%B4%AD%E4%B9%B0%E7%9A%84%E5%9F%9F%E5%90%8D%EF%BC%8C%E7%82%B9%E5%87%BB%E5%8A%A0%E5%85%A5%E6%B8%85%E5%8D%95%EF%BC%8C%E5%86%8D%E7%82%B9%E5%87%BB%E7%AB%8B%E5%8D%B3%E7%BB%93%E7%AE%97%E3%80%82)
购买完之后，记得等待两到三天，域名备案，备案步骤比较简单，此处不再张贴相关网址。有需要可以自行百度。
（当然了如果你不想要备案，可以自行网上搜索资源购买外网服务器-建议大家遵守国家法律）
阿里云域名备案网站链接：
[https://beian.aliyun.com/](https://beian.aliyun.com/)
> 在阿里云备案完成后会收到阿里云客服电话 
一天之内在下面网站填写收到的短信验证码

具体操作看下图
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1694483871727-9dd24605-dcce-4877-ba1f-c3fe94e17a25.png#averageHue=%23d7deb0&clientId=u6a898266-bd7f-4&from=paste&height=827&id=uf4e01582&originHeight=930&originWidth=1910&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=437463&status=done&style=none&taskId=u34ce0458-b4be-4c53-9141-838c80e5686&title=&width=1697.7777777777778)
工业和信息化部政务服务平台
[https://beian.miit.gov.cn/#/Integrated/index](https://beian.miit.gov.cn/#/Integrated/index)
## 域名配置
域名DNS解析参考链接
[https://blog.csdn.net/fate_sky8521/article/details/116610662](https://blog.csdn.net/fate_sky8521/article/details/116610662)
阿里云DNS解析链接直达
[https://dc.console.aliyun.com/next/index?spm=5176.28261954.J_7341193060.3.18a62fdeXd56ej#/domain-list/all](https://dc.console.aliyun.com/next/index?spm=5176.28261954.J_7341193060.3.18a62fdeXd56ej#/domain-list/all)
开始前记得先在阿里云或其他云平台进行域名解析
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1695197473415-7d50a972-eba5-40b2-a037-71cea69c7c89.png#averageHue=%23c7a994&clientId=ue523ea05-ddde-4&from=paste&height=610&id=u233b5490&originHeight=762&originWidth=1601&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=289957&status=done&style=none&taskId=ufca7014b-16d1-4c4b-ab45-27f941a4cec&title=&width=1280.8)
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1695197568352-398bc652-dadf-4cd4-9037-4c359db603d8.png#averageHue=%23f0f0ef&clientId=ue523ea05-ddde-4&from=paste&height=623&id=u4d4a52bb&originHeight=779&originWidth=1580&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=211816&status=done&style=none&taskId=ufc2ac689-25e4-4dc1-9a62-a1daf7cbbc8&title=&width=1264)
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1695197730805-a93ae908-9909-4d78-ac5f-35a683e5becb.png#clientId=ue523ea05-ddde-4&from=paste&height=702&id=uf9410877&originHeight=877&originWidth=931&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=61313&status=done&style=none&taskId=u1ce07667-4be9-470f-9806-a6ee7b029b8&title=&width=744.8)
验证你的域名解析是否成功
可以在终端控制台ping下就行
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1695197822149-27779b13-1a16-4d53-8173-394d90443e5b.png#clientId=ue523ea05-ddde-4&from=paste&height=260&id=u0043d177&originHeight=325&originWidth=971&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=45508&status=done&style=none&taskId=u7f821c58-bd38-463f-aa3f-c4f7dc9d43c&title=&width=776.8)

## 域名CA证书实战
标题，这是一个让你的域名访问协议由http变为https的方法。
想要了解原理的访问我的这篇公众号推文
[https://mp.weixin.qq.com/s/csnMjdI1NYtCzFEgSQp7xw](https://mp.weixin.qq.com/s/csnMjdI1NYtCzFEgSQp7xw)
### 宝塔方式
CA证书配置有两种方式，一种是宝塔直接下面页面申请即可。另一种是阿里云（或者其他云平台或其他CA证书认证平台）
注：宝塔有缺陷，CA证书可能只能用3个月（这个不太清楚，待实践，因为我用的阿里云的免费证书，直接一年）。
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1695177167281-b546319c-e635-4462-991e-8e522cbbdbf5.png#averageHue=%23faf9f8&clientId=u24b85f30-a030-4&from=paste&height=580&id=B2CeY&originHeight=725&originWidth=816&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=56869&status=done&style=none&taskId=ucd181757-37a8-4b49-ac6f-da24b9d1fa6&title=&width=652.8)
然后当前证书页面会生成KEY和PEM,直接保存即可，保存完之后点击强制HTTPS按钮。
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1695196775627-8359fb59-4213-47dc-8b34-019010f0ad5e.png#averageHue=%23dfd6cb&clientId=ue523ea05-ddde-4&from=paste&height=571&id=ue3fafe3b&originHeight=714&originWidth=852&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=75510&status=done&style=none&taskId=u3760a03f-3d7f-426d-a9f5-603fe29c62e&title=&width=681.6)
### 阿里云方式
#### CA证书领取
阿里云免费证书直达链接
https://common-buy.aliyun.com/?commodityCode=cas#/buy
先领取证书资源包，看下图
![](https://cdn.nlark.com/yuque/0/2023/png/38420467/1695024903706-0ed34ce1-6979-4586-bb54-b007a04e4514.png#averageHue=%23fdfbfa&clientId=u980c851e-7031-4&from=paste&id=u405306b5&originHeight=413&originWidth=1080&originalType=url&ratio=1.125&rotation=0&showTitle=false&status=done&style=none&taskId=u54b535e1-73ab-4cee-8ec9-cc4143389ff&title=)
然后在控制台配置，域名证书即可，因为可以领取20个证书资源包，所以应该可以配置20个网站为https协议
过程时间很快5-10分钟
#### CA证书配置
阿里云直达链接
[https://yundun.console.aliyun.com/?spm=5176.7968328.J_8413632810.1.418365c33GdGH3&p=cas&showBuy=1#/certExtend/free/cn-hangzhou](https://yundun.console.aliyun.com/?spm=5176.7968328.J_8413632810.1.418365c33GdGH3&p=cas&showBuy=1#/certExtend/free/cn-hangzhou)
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1695118720729-981c9d61-17b0-4adb-af49-a015ed80eb44.png#averageHue=%23fdfbfb&clientId=ubb439d8f-0e33-4&from=paste&height=460&id=u893ea4b1&originHeight=575&originWidth=1642&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=80078&status=done&style=none&taskId=ub8ce27a3-648f-41f5-ae35-7881a50fecf&title=&width=1313.6)
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1695118595710-1ced1fdd-9d85-4e5e-b0ee-3a5993b94feb.png#averageHue=%23faf9f7&clientId=ubb439d8f-0e33-4&from=paste&height=693&id=u951bd414&originHeight=866&originWidth=1091&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=87737&status=done&style=none&taskId=u2a2bad6a-4250-4589-b4b1-696001f435a&title=&width=872.8)
由于我使用的是宝塔部署的网站，所以必须将数字证书下载到本地。
下载完后，将解压会得到一个pem和key文件，这个是我们要用的，可以选择使用本地记事本打开
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1695024350976-c0a2b097-6165-4a3f-bd36-c3fd15bb9271.png#averageHue=%23fcfbfb&clientId=u980c851e-7031-4&from=paste&height=804&id=u1ea89278&originHeight=905&originWidth=1910&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=140354&status=done&style=none&taskId=ub2ede33e-5bcd-4294-bb18-7add279e274&title=&width=1697.7777777777778)
选择你对应的网站代理服务器类型，我得服务器类型是nginx所以我这里选择nginx
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1695025119707-03f558e5-ed43-4062-8e68-ec1882550a74.png#averageHue=%23deb581&clientId=u980c851e-7031-4&from=paste&height=729&id=d6QXv&originHeight=820&originWidth=1084&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=51872&status=done&style=none&taskId=u4a64a752-5b9d-4204-90bb-adc3632785f&title=&width=963.5555555555555)
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1695024668797-8aba7be9-da38-483e-8d7d-562267c3c7c5.png#averageHue=%23f6f6f5&clientId=u980c851e-7031-4&from=paste&height=667&id=u7b2359c6&originHeight=750&originWidth=1026&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=132628&status=done&style=none&taskId=u106feb15-3196-49e7-a087-35a7cda5af9&title=&width=912)
然后粘贴到宝塔SSL页面即可。
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1695024587914-95911a02-fa00-45b0-8cbf-9ea1e126820e.png#averageHue=%23eef1e9&clientId=u980c851e-7031-4&from=paste&height=805&id=ud71ca3d8&originHeight=906&originWidth=997&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=110764&status=done&style=none&taskId=u519d0011-3e2b-4e1d-bddf-fbd0654fc35&title=&width=886.2222222222222)

完结
前端后端，我都进行了https协议加密。有兴趣的小伙伴也可以尝试下哦！
展示图
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1695197965226-98de7e71-32e2-4b75-ab16-04b6f9d04acc.png#averageHue=%230f150f&clientId=ue523ea05-ddde-4&from=paste&height=763&id=ud52d6f60&originHeight=954&originWidth=1912&originalType=binary&ratio=1.25&rotation=0&showTitle=false&size=1523008&status=done&style=none&taskId=u158e06be-d3bb-471b-8446-fb6e2705e66&title=&width=1529.6)
大家有兴趣的可以拜访下我的小破网站
[https://techmindwave.nanchengyu.cn/](https://techmindwave.nanchengyu.cn/)
服务器不太行，大家轻点搞。哈哈哈哈~
