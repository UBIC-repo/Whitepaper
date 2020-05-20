# 目录

- [全民基本收入](#全民基本收入)
- [前期研究和其他项目](#前期研究和其他项目)
- [经济体制](#经济体制)
- [防御女巫攻击](#防御女巫攻击)
- [共识](#共识)
- [电子护照](#电子护照)
- [数字签名的不可转移性](#数字签名的不可转移性)
- [地址结构](#地址结构)
- [交易/事物](#交易事物)
- [区块](#区块)
- [可能的问题](#可能的问题)
- [其他应用场景](#其他应用场景)

# 全民基本收入

当前的加密货币的奖励体系中，都是通过工作量证明（POW）或权益证明（POS）将奖励分配给保障网络安全运行的矿工，但对于网络的参与者并没有任何奖励。
现有的奖励机制将会导致网络参与者之间有着非常不均衡的奖励分配，由此UBIC提出了一种新的加密货币体系，所有参与者通过全民基本收入（UBI）来获得奖励。

# 前期研究和其他项目

截止2020年，在互联中已经存在数千种加密货币，UBIC并不是第一个旨在实现全民基本收入（UBI）发行的项目。非UBI和UBI加密货币的主要区别在于需要解决女巫（sybil）攻击。

例如，一些类似于 "Duniter" 的项目，已经开始建立一个需要用户彼此“验证”的“信任网络”。想法虽然很简单，但是建立一个“信任网络”实际上是非常复杂的，需要进行先进的图论算法加人工验证。另一种方法是针对参与者进行图灵测试---例如：“Idena”使用翻转难题对参与
者进行验证，这将消耗参与者大量的时间，并且对于能否抵抗人工智能学习依旧是一个长期的挑战。

UBIC尝试通过另一种方法来解决此问题，该方法利用信息差距较小的现代电子护照提供的近场通信（NFC）芯片进行验证。

# 经济体制

无限供应的货币或许没有任何什么价值，这就是为什么每年的发行总量是固定的。
不同的货币运行在一个独特的区块链上，每种货币与一个国家/地区关联，并按照"U" + 国家/地区对应ISO 3166-2代码命名，例如：UCH 代表瑞士的货币， UDE 代表德国， UAT 代表奥地利 以及 UUK 代表英国。
区块产出很大一部分将平均分配给成功与护照关联的地址，以UCH为例，如果瑞士的UBIC货币每块产出100个并且有50本瑞士护照完成注册验证，每本护照所关联的地址将获得2UCH。一段时间后，瑞士有500本完成注册验证的护照，区块产出仍然是每块产出100个或多一点，每本护照所关联的地址将获得0.2UCH。

下列表格显示了每个国家/地区UBIC货币的发行数量。

| 货币代码 | 国家/地区  | UBI 每年发行数量 | 附加信息
| :---- | :--------- | :---------------- | :------------- |
| UCH  | 瑞士              | 10,196,640  |  | 
| UDE  | 德国                  | 100,599,840   |  | 
| UAT  | 奥地利                   | 10,617,120  | 2014年10月后的护照 | 
| UUK  | 英国          | 79,838,640  |  | 
| UIE  | 爱尔兰                   | 5,781,600 |  2016年5月后的护照 | 
| UUS  | 美国                      | 393,096,240   |  | 
| UAU  | 澳大利亚               | 29,223,360  |  | 
| UCN  | 中国                   | 1,677,767,760   | 2019年7月以后的香港护照
| USE  | 瑞典                  | 12,036,240  |  | 
| UFR  | 法国                  | 81,730,800  |  | 
| UCA  | 加拿大                  | 44,150,400  |  | 
| UJP  | 日本                   | 154,526,400   | 2016年5月以后的护照 | 
| UTH  | 泰国                  | 81,520,560 |  | 
| UNZ  | 新西兰               |  5,571,360 |  | 
| UAE  | 阿拉伯联合酋长国    | 11,300,400 |  | 
| UFI  | 芬兰                   | 6,675,120 |  | 
| ULU  | 卢森堡               | 525,600       | | 
| USG  | 新加坡               | 6,832,800   | | 
| UHU  | 匈牙利                   | 11,931,120  | | 
| UCZ  | 捷克共和国            | 12,877,200  |  | 
| UMY  | 马来西亚                  | 38,684,160  |  | 
| UUA  | 乌克兰                   | 54,767,520  |  | 
| USP  | 西班牙                   | 108,000,000   | 2016年7月以后的护照 |
| UHK  | 香港                  | 17,100,000  | 2019年7月以后的护照 | 
| UIS  | 冰岛                   | 420,480   | 2013年2月以后的护照 |
| UEE  | 爱沙尼亚                   | 1,681,920   | 暂无注册 | 
| UMC  | 摩纳哥                  | 52,560  | 暂无注册 | 
| ULI  | 列支敦士登           | 52,560  | 暂无注册 | 
| UIS  | 冰岛           | 420,480   | 2013年2月之后的护照
| UHK  | 香港           | 8,988,000   | 暂无注册
| UES  | 西班牙           | 56,764,800  | 2016年7月之后的护照
| URU  | 俄罗斯          | 
| UIL  | 以色列          | 
| UPT  | 葡萄牙          | 
| UDK  | 丹麦           | 
| UTR  | 土耳其          | 
| URO  | 罗马尼亚           | 
| UPL  | 波兰          | 

*表格中显示的数字是最大数字，假设每分钟铸造一个方块

# 额外分配
除了上述发行量外，验证器节点还铸造了10％的货币。
开发基金收取10％的额外奖励，且每525600个区块减半，直到最终达到1.25％。

# 防御女巫攻击

UBIC使用现代电子护照的安全功能抵抗女巫攻击. 您可以使用近场通信（NFC）读取现代电子护照加入UBIC. 得益于不可以转移的签名技术，
您的身份并不会因此泄漏，因为您的护照只有唯一的哈希值存储在区块链上，下一章节会进行更详细的解释。

截至目前，UBIC可以在28个国家/地区使用，一些国家已完全满足UBIC对电子护照的安全要求，以确保能够防御女巫攻击。一旦其他国家/地区
支持UBIC对电子护照的安全要求，UBIC可能会有更多的国家/地区的参与者加入。


# 电子护照
过去十年来，已经有许多国家发行了电子护照，有时我们也称之为生物特征护照。
这些护照通过近场通信（NFC）和加密算法提供了更强的安全性，几乎无法进行伪造。
电子护照是根据国际民用航空组织(ICAO)编写的护照9303标准（DOC9303）制作，因此所有的电子护照都必须实现这些特性。
但由于每个国家/地区可以自由选择加密算法，其中一些国家/地区的加密强度还未达到UBIC的要求（例如：香港在2019年6月之前使用3位的RSA公钥指数，而UBIC需要大于65537位的RSA公钥指数），这就是为什么不是所有的护照都能在UBIC中使用的原因。

### 近场通信（NFC）芯片
电子护照中最关键的部分就是嵌入其中的NFC芯片，该芯片通常存储了分布在多个数据组中的32-64kb的信息：
 - 数据组1将名、姓、出生日期和到期日期等信息存储在机器可读区（Machine Readable Zone），通常简称为机读区。
 - 数据组2存储面部图像。
 - 数据组3存储指纹信息，只能使用名为“扩展访问控制”的机器来访问它，该“扩展访问控制”机器的控制权仅有政府持有。
最后，在文档安全对象中有一个PKCS7文件，其中存储了使用政府颁发的文档签名证书对所有数据组进行签名的哈希。
UBIC仅读取文档安全对象，用于生成无法篡改的数字签名。

### 基础访问权限
使用近场通信（NFC）技术可以读取最远10厘米范围内的无源标签。从理论上来讲，你可以利用此技术从某个人的口袋里读出他的护照。
但是，由于被称为“基本访问控制”的安全功能，这并不容易。如果护照启用了此功能，则护照号码、出生日期和有效日期就像密码一样，你必须提供给NFC芯片这三个信息以读出内容。

### 文档签名证书
根据国际民用航空组织编写的护照9303标准（DOC9303）规定，文档签名证书至少每三个月重新颁发一次，且签名时间有限，此后应当销毁其私钥。
这样可以确保如果一个文档签名证书被滥用，则只需要重新签发少量的护照，所有文档签名证书必须由国家签名证书颁发机构签名颁发。
 
### 国家签名证书
国家签名证书由国家签名证书颁发机构（CSCA）签名颁发，该证书在政府公钥基础设施中拥有最高级别的特权。

### 公钥目录（PKD）
公钥目录是一个由国际民用航空组织公开的国家签名证书和文档签名证书公钥的目录。
下载链接是: https://pkddownloadsg.icao.int/
公钥目录并不是唯一可以获得这些证书来源的地方，一些政府发布了它们的国家签名证书，以及他们信任的其他国家/地区的证书，
文档签名证书也可以在护照上被找到，这也就是我们为什么没有支持所有国家护照的原因之一。

# 数字签名的不可转移性
数字签名的不可转移性是UBIC能够通过一种安全而体面的方式验证UBIC地址与未知真实护照之间联系的关键，这项技术可以在不透露数字签名信息的情况下进行验证。
 
### ECDSA算法
#### 生成签名
我们定义 ![m](https://github.com/UBIC-repo/images/raw/master/formulas/m.png) 为护照信息的哈希， ![R](https://raw.githubusercontent.com/UBIC-repo/images/master/formulas/R.png) 为从签名中提取的椭圆曲线点 ![(r,s)](https://raw.githubusercontent.com/UBIC-repo/images/master/formulas/rs.png)
将在区块链上显示出:

 - ![](https://github.com/UBIC-repo/images/raw/master/formulas/m.png)

 - ![](https://raw.githubusercontent.com/UBIC-repo/images/master/formulas/R.png)

 - ![](https://raw.githubusercontent.com/UBIC-repo/images/master/formulas/Qpa.png) 例如 ![](https://raw.githubusercontent.com/UBIC-repo/images/master/formulas/QapsR.png) 

 - ![](https://raw.githubusercontent.com/UBIC-repo/images/master/formulas/Rp.png) 例如 ![](https://raw.githubusercontent.com/UBIC-repo/images/master/formulas/rpkpr.png) 其中 ![](https://raw.githubusercontent.com/UBIC-repo/images/master/formulas/kp.png) 是一个随机数.

 - ![](https://raw.githubusercontent.com/UBIC-repo/images/master/formulas/sp.png) 例如 ![](https://raw.githubusercontent.com/UBIC-repo/images/master/formulas/spk1mprps.png) 并且其中 ![](https://raw.githubusercontent.com/UBIC-repo/images/master/formulas/mp.png) 是获得奖励的UBIC地址。

#### 验证

 - 步骤1. 验证 ![](https://raw.githubusercontent.com/UBIC-repo/images/master/formulas/verif1.png)

 - 步骤2. 验证 ![](https://raw.githubusercontent.com/UBIC-repo/images/master/formulas/verif2.png)

### RSA算法
#### 生成签名
我们定义 ![](https://raw.githubusercontent.com/UBIC-repo/images/master/formulas/X.png) 为护照信息的哈希， ![](https://raw.githubusercontent.com/UBIC-repo/images/master/formulas/e.png) RSA指数通常是 ![](https://raw.githubusercontent.com/UBIC-repo/images/master/formulas/2161.png) 和 ![](https://raw.githubusercontent.com/UBIC-repo/images/master/formulas/A.png) 进行签名，然后根据Guillou-Quisquater协议证明A的解决方案是:

 - ![](https://raw.githubusercontent.com/UBIC-repo/images/master/formulas/e.png) RSA指数通常是 ![](https://raw.githubusercontent.com/UBIC-repo/images/master/formulas/2161.png) 
 - ![](https://raw.githubusercontent.com/UBIC-repo/images/master/formulas/X.png) 护照信息的哈希。
 - ![](https://raw.githubusercontent.com/UBIC-repo/images/master/formulas/t1..5eAd1..5r.png) 其中d是从UBIC公钥推导的16位带盐哈希，r是一个加密的随机数
 - ![](https://raw.githubusercontent.com/UBIC-repo/images/master/formulas/T.png) 例如 ![](https://raw.githubusercontent.com/UBIC-repo/images/master/formulas/Tre.png)

因为 1 < d < e 并且e通常等于 ![](https://raw.githubusercontent.com/UBIC-repo/images/master/formulas/2161.png) 上述操作必须用不同的d值进行多次，在当前的UBIC实现中至少会进行5次。

#### 验证

 - ![](https://raw.githubusercontent.com/UBIC-repo/images/master/formulas/t1..5vXd1..5T.png)

在验证生成的过程中，每生成一个d值，均需重复上述操作。

# 地址结构
UBIC的地址是base58格式的二进制数据，地址结构如下:
```
<程序标识符> <负载长度> <负载内容> <校验和>
      1 byte             1-4 bytes     x bytes   3 bytes
```

程序标识符使UBIC能够更加轻松的升级和添加新的功能，例如用于智能合约的新脚本语言。

例子:
```
<程序标识符> <负载长度>                   <负载内容>                      <校验和>
       0x02                0x14         0x23be5a8564ebc151004d798ef812aa25ee7ff79        0x23f234
```
```0x02``` 是使用 ```ripemd160((sha256(public key))``` 进行哈希处理以进行哈希支付的程序标识符。

```0x14``` 是20的十六进制表示，ripemd160的长度。

```0x23be5a8564ebc151004d798ef812aa25ee7ff79``` 是负载内容， 在此情况下为公钥的哈希。

```0x23f234``` 是通过以下计算从结果中取前3个字节获得的校验和 ```sha256(<程序标识符> <负载长度> <负载内容>)```

我们不需要为每一种货币创建不同的地址，一个地址即可接收、持有和发送所有UBIC货币。

# 交易/事物

### 结构
交易可以有1个/多个或者0个/1个或多个输出，但输入值必须大于或等于输出值。
为了减少通货膨胀，sum(inputs) - sum(outputs)将作为交易消耗的费用并销毁。
一次交易可以转移多种货币。但是你无法将一种货币转换为另外一种货币。

### 交易标准
标准的交易结构如下:
- network（网络）
- txIns（输入）
	- amount（金额）
	- inAddress（输入地址）
	- nonce（随机数）
	- script（脚本）
- txOuts（输出）
	- amount（金额）
	- script（脚本）

network ：是一个 ```uint8_t``` 字段, 它确保来自测试网络的交易不会被广播到主网。
nonce   ：是一个 ```uint32_t``` 字段, 它确保交易无法被多次广播。
amount  ：是一个将货币编号 (```uint8_t```) 映射到货币金额 (```uint64_t```)的字段。
script  ：是一个 ```std::vector<unsigned char>``` 字段，它包含了一个序列化对象。

### 共识货币兑换
假如 Alice 拥有10 UCH并想和 Bob 交换10 UDE，他们可以以此为目的达成链上共识交易。
假如 Alice 的地址是 0x17a6 ，Bob 的地址是 0x98b1。 那么本次交易输入0x17a6(10 UCH)， 0x98b1(10 UDE) 并同时输出0x17a6(10 UDE), 0x98b1(10 UCH)
以达成他们的目的。
 
# 区块
区块结构如下:
- BlockHeader（区块头）
  - version（版本）
  - headerHash（哈希头）
  - previousHeaderHash（上个哈系头）
  - merkleRootHash（默克尔根哈希）
  - blockHeight（区块高度）
  - timestamp（时间戳）
  - payout（支付）
  - payoutRemainder（支付金额）
  - ubiReceiverCount（计数器）
  - votes（投票票数）
  - issuerPubKey（发行人公钥）
  - issuerSignature（发行人签名）
- Transactions（交易）

# 共识
UBIC没有矿工, 而是由委托人验证区块。8位由中央控制的创世代表将在早期为网络提供验证支持。随着时间的流逝，新的代表将代替创世代表，
从而使UBIC真正地分散。代表的增减将通过代表投票决定，代表可以是人、公司、非盈利组织或任何能够运行节点并愿意支持此项目的实体。
他们将由社区制定，然后由其他代表投票表决。如果有代表行为不当，则其他代表应当取消投票来取消其代表权限。

# 可能的问题
### 持有多个护照的人
出于隐私原因，UBIC不会将任何个人信息传输到区块链。 UBIC假设每个人只有一本有效护照，但事实并非如此。
人们可以在旧护照过期或护照被盗后申领新的护照。
因为护照的吊销清单不是公开的，所以UBIC假设所有未到达护照有效期的护照都是有效的。
有些人最终可能获得了2或3个经过验证的有效地址，但他们不太可能获得更多。.
有一些因素可以减轻这种风险:
 - 真正的护照在黑市上价值几千美元，这就是为什么如果有人经常“丢失”他/她的护照，他/她将很难获得新的护照并且会引起执法部门的注意。
 - 领取新护照所需的费用和时间可能会超过获得更多UBIC的好处。
 - 政府可以签名并公开护照吊销清单，被盗或丢失的护照将立即停止接受的UBIC
 
### 威胁
政府可能对这种加密货币怀有不同的想法。它们可以尝试通过立法或黑客的手段攻击它。由于政府可以发放文档签名证书，它们可以通过注册大量护照滥用网络，但这似乎不太可能，因为这样会损害它们的信誉。
 
### 隐私问题
虽然非政府机构很难通过地址找到其真实身份，但颁发护照的政府肯定可以这样做。
 
# 其他应用场景
### 了解你的客户（KYC）
虽然区块链本身并没有存储任何个人信息, 但用户可以决定将数据组1和数据组2中包含的信息透露给其他实体，来进行身份验证。

### 投票
UBIC可能有两种方案，在第一轮的投票中，投票者使用持有的货币对其进行加权，就像许多现有的加密货币一样。
在第二种方案中，只有UBIC的接收者才能以一个接收者一票的权重进行投票，因为投票者的国家/地区是已知的，
所以投票也可以针对特定国家/地区进行。
