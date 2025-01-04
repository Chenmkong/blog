# Headline

> An awesome project.

                                       SAP用户手册

[TOC]

# 1.  SAP登录

## 1.1  新建连接

![](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240729203453438.png)<img src="C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240729203707062.png" alt="image-20240729203707062" style="zoom: 30%;" /><img src="C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240729210339853.png" alt="image-20240729210339853" style="zoom:33%;" /><img src="C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240729212721007.png" alt="image-20240729212721007" style="zoom: 40%;" /><img src="C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240729213008541.png" alt="image-20240729213008541" style="zoom: 50%;" />

## 1.2  登录

![image-20240729213321404](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240729213321404.png)<img src="C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240729214622160.png" alt="image-20240729214622160" style="zoom:33%;" />

![image-20240731193441576](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240731193441576.png)

### 1.2.1  导航区显示T-CODE

*菜单栏 → 附加 → 设置 →显示技术名称*

 ![image-20240731203615622](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240731203615622.png)

```
技术名称：具有唯一性，可以是T-CODE,字段名，系统标识  
文本描述：可以重复
```

### 1.2.1  设置本地布局

![image-20240731201519828](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240731201519828.png)![image-20240731201625972](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240731201625972.png)![image-20240731201747840](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240731201747840.png)

### 1.2.3  设置个人数据

*SU3:菜单栏 → 系统→ 用户参数文件 → 个人数据*

![image-20240731204213235](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240731204213235.png)![image-20240731204450964](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240731204450964.png)

然后点击保存，退出重新登录后生效

### 1.2.4  常用T-CODE

```
SU3:个人信息设置
SPRO  后台设置
/N  回到前台
/N TCODE 关闭当前打开新的
/O 新建窗口
/O TCODE在新窗口打开业务场景
```



# 2 FI模块

## 2.1 GL  

### 2.1.1  建立组织架构

#### 设置IMG附件信息

*路径：SPRO→设置→用户特定的（E）→IMG结构→IMG活动ID*

![](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240807201542686.png) ![image-20240807201653534](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240807201653534.png)

设置好后IMG右侧会有附件信息显示![image-20240807201827609](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240807201827609.png)

#### 定义公司

此公司不是公司代码，可以理解为**贸易伙伴**，用于跨公司交易的标识，用于公司间的资产调拨。。

*路径：SPRO→![image-20240807202315974](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240807202315974.png)→企业结构→定义→财务会计→定义公司(SM12-删除用户-列表-删除所有：可解锁其他用户的锁定状态)→新条目*

![image-20240807202505229](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240807202505229.png)

![image-20240807204006191](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240807204006191.png) 

![image-20240807204455172](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240807204455172.png) 

以上配置好后→保存→创建请求→简短描述→保存

![image-20240807205205231](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240807205205231.png)

![image-20240807205529477](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240807205529477.png) 

下面是最后的显示，然后✔就行了![image-20240807205759538](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240807205759538.png) 

#### 定义信贷控制范围

目的：控制赊销业务

*路径：SPRO→![image-20240807202315974](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240807202315974.png)→企业结构→定义→财务会计→定义信贷控制范围→* 

![image-20240808134416361](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808134416361.png)

 *点击![image-20240808134622002](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808134622002.png)*

![image-20240808135436220](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808135436220.png) 

*设置好后点保存*

![image-20240808135549047](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808135549047.png)

#### 编辑，复制，删除，检查公司代码

##### 创建总公司

![image-20240808135900332](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808135900332.png) 

![image-20240808140105207](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808140105207.png) 

![image-20240808140750635](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808140750635.png) 

![image-20240808140528778](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808140528778.png) 

![image-20240808140635425](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808140635425.png) 

![image-20240808140703179](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808140703179.png) 

##### 创建分公司（通过复制功能）

选中要复制的公司代码后，点赋值为![image-20240808141635423](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808141635423.png) 

修改公司代码和名称后点 回车

 ![image-20240808141805757](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808141805757.png)

修改名字![image-20240808141940905](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808141940905.png) 

创建子公司0316（同样逻辑创建）

操作结束后点保存 

![image-20240808142322501](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808142322501.png)

#### 给公司/信贷控制范围分配公司代码

![image-20240808142727180](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808142727180.png) 

![image-20240808142911125](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808142911125.png) 

![image-20240808142937602](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808142937602.png) 

![image-20240808143023840](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808143023840.png) 

### 2.1.2  创建科目表

#### 创建总分公司科目表

![image-20240808144131447](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808144131447.png) 

![image-20240808144424048](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808144424048.png) 

创建子公司科目表（通过复制创建）

![image-20240808144815761](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808144815761.png) 

#### 给科目表分配公司代码

![image-20240808145305203](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808145305203.png) 

![image-20240808145511220](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808145511220.png) 

#### 定义科目组

![image-20240808145753854](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808145753854.png) 

![image-20240808150118802](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808150118802.png) 

定义科目组的字段状态：控制科目主数据

![image-20240808150921184](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808150921184.png) 

![image-20240808150840400](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808150840400.png) 

![image-20240808151205091](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808151205091.png)

![image-20240808151219670](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808151219670.png) 

#### 定义留存收益科目

![image-20240808151505239](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808151505239.png) 

![image-20240808151651761](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808151651761.png) 

这里的账户并没有实际创建，所以点保存时会出现黄色警告。这时候点回车。

![image-20240808152139073](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808152139073.png) 

#### 定义字段状态组：控制凭证行项目

![image-20240808152516525](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808152516525.png) 

![image-20240808152622684](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808152622684.png) 

![image-20240808153933019](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808153933019.png) 

![image-20240808154117474](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808154117474.png) 

点击新条目![image-20240808154140278](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808154140278.png) 

![image-20240808154825435](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808154825435.png)  

![image-20240808155732736](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808155732736.png) 

![image-20240808155755292](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808155755292.png) 

![image-20240808155818219](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808155818219.png) 

**字段状态组分配给公司代码**

![image-20240808160144669](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808160144669.png) 

![image-20240808160357010](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808160357010.png) 

#### 维护会计年度变式

![image-20240808160536368](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808160536368.png) 

![image-20240808161350499](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808161350499.png) 

**会计年度变式分配给公司代码**

![image-20240808161447724](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808161447724.png)

![image-20240808161603023](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808161603023.png) 

#### 创建会计科目

FS00

![image-20240808162346182](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240808162346182.png) 

![image-20240810131826450](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240810131826450.png) 

![image-20240810131902473](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240810131902473.png) 

### 2.1.3  总账业务数据配置

#### 凭证号范围设置：

<u>编号类的设置需要手工进行传输</u>

OBH1:将模板公司凭证编号复制到公司代码

![image-20240813092033597](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240813092033597.png) 

![image-20240813092230531](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240813092230531.png) 

OBH2 公司代码的凭证编号复制到会计年度：年结动作

![image-20240813092328953](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240813092328953.png) 

![image-20240813092422909](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240813092422909.png) 

编号范围状态会自动储存最后一个使用的凭证号

![image-20240816113317526](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240816113317526.png) 

FBN1 查询编号范围，如果勾选了外部，则手工编号，一般财务模块不用

![image-20240813092703633](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240813092703633.png) 

#### 容差组

##### 总账容差组OBA0

命名时空白，SAP空白时，默认分配给科目里了。

![image-20240813095516083](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240813095516083.png) 

![image-20240813095809304](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240813095809304.png) 

![image-20240813100942445](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240813100942445.png) 

##### 雇员容差组

- 针对SAP用户设置的容差组
- 参照总账容差就可以了

![image-20240815191345565](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815191345565.png) 

##### 定义总账容差科目（表外科目）

![image-20240815191005508](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815191005508.png) 

进去后先点保存

![image-20240815200012807](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815200012807.png) 

FS00建立总账差异科目55039100

![image-20240815200519460](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815200519460.png) 

![image-20240815200643857](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815200643857.png) 

返回容差科目设置填入55039100

![image-20240815200734574](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815200734574.png) 



#### OB52 打开关闭会计期间 月结动作

定义未结清过账期间变式

![image-20240815202038378](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815202038378.png) 

![image-20240815202213483](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815202213483.png) 

分配给公司代码

![image-20240815202329807](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815202329807.png) 

![image-20240815202359066](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815202359066.png) 

OB52

![image-20240815202927278](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815202927278.png)  

![image-20240815203346885](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815203346885.png) 

结算8月的账时，打开9月期间

![image-20240815203817066](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815203817066.png) 

结算完后，关闭8月

![image-20240815203937369](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815203937369.png) 

特殊期间

![image-20240815204045384](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815204045384.png) 

+所有，A资产，D客户，K供应商，M物料,S总账

#### 定义成本控制范围

OKKP

![image-20240815212852600](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815212852600.png) 

![image-20240815213003967](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815213003967.png) 

![image-20240815213103629](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815213103629.png) 

![image-20240815213131953](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815213131953.png) 

![image-20240815213427816](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815213427816.png) 

然后点击新条目

![image-20240815213604184](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815213604184.png) 

#### 定义分类账和货币设置

![image-20240815214413668](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815214413668.png) 

![image-20240815214546533](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815214546533.png) 

检查有没有这两个，没有的话，维护上，然后点保存。

![image-20240815214627601](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815214627601.png) 

同样的操作，去操作OC和OE

![image-20240815214907186](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815214907186.png) 

#### 定义CO版本的分类账

![image-20240815215252256](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815215252256.png) 

进去后添加新条目

![image-20240815215423900](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815215423900.png) 

#### 激活凭证分解

![image-20240815215623264](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815215623264.png) 

![image-20240815215731117](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815215731117.png) 

![image-20240815215838402](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815215838402.png) 打勾保存

### 2.1.4  F-02做一个凭证

![image-20240815222914647](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240815222914647.png) 

FB03

![image-20240816131957176](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240816131957176.png) 

# 3.  数据批量导入

导入静态前，需要先删除业务数据；

OBR1:删除业务数据 OBR2：删除主数据

## 1.1  科目主数据导入

### a.  数据删除

OBR1删除业务数据

![image-20240901100121122](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901100121122.png) 

OBR2删除会计科目

![image-20240901100649576](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901100649576.png) 

### b.  关闭FS00导航树

![image-20240901101236197](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901101236197.png) 

### c.  LSMW

![image-20240901101812635](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901101812635.png) 

![image-20240901101848338](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901101848338.png) 

![image-20240901101922713](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901101922713.png) 

![image-20240901102056169](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901102056169.png) 

![image-20240901102214530](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901102214530.png) 

#### 1.定义对象属性

主数据导入使用录屏方式

![image-20240901102347411](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901102347411.png) 

![image-20240901102915411](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901102915411.png) 

![image-20240901103100623](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901103100623.png) 

![image-20240901103148279](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901103148279.png) 

![image-20240901103227793](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901103227793.png) 

模拟创建会计科目的步骤：可能使用的字段上要有数据，这样SAP的录屏就能识别出步骤了

![image-20240901103509407](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901103509407.png) 

![image-20240901103809534](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901103809534.png) 

![image-20240901104246230](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901104246230.png) 

![image-20240901104616727](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901104616727.png) 

![image-20240901105050399](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901105050399.png) 

![image-20240901105139584](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901105139584.png) 

![image-20240901105335404](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901105335404.png) 

![image-20240901105445181](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901105445181.png)  

![image-20240901105542915](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901105542915.png) 

![image-20240901105617563](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901105617563.png) 

![image-20240901105708307](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901105708307.png) 

# 4  ARAP

**维护BP编号范围**

常用的是02和AB，02流水号，AB外部给号，可数字可字母

![image-20240901144307737](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901144307737.png) 

**BP编号分组**

![image-20240901144632905](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901144632905.png) 

**供应商/客户分组**

屏幕格式就是指字段状态组

![image-20240901145025634](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901145025634.png) 

账户组的维度：集团内外，国内外，财务专用供应商（指不走PO,SO），员工供应商（发工资），一次性供应商（一锤子买卖，通过同一个编码管理若干个供应商）

![image-20240901145625129](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901145625129.png) 

供应商/客户分组编号 都选上外部给号，系统过会根据BP号码通过主数据同步，将三个编号统一

**将编号分给供应商/客户组**

**主数据同步**

![image-20240901150423211](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901150423211.png) 

![image-20240901150448934](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901150448934.png) 

![image-20240901150516930](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901150516930.png) 

![image-20240901150535666](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901150535666.png) 

**BP**

先创建000000角色

![image-20240901153057640](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901153057640.png) 

**双重敏感字段**

供应商的联系方式，银行卡号等敏感信息可以设置成有权限的修改才有用



物料主数据MM01

供应商主数据BP

采购信息记录ME11

PR ME51N

PO ME21N

收货 MIGO  DR：存货(BSX)  Cr：GR/IR(WRX,GRIR是在途物资和应付暂估的含义）

发票校验 MIRO  Dr：GR/IR,进项税  Cr:应付账款

财务付款F-53 Dr:应付账款 Cr:银行存款

**GR/IR重分类**

GR/IR是表外科目，如果月结有余额，需要在月末使用**F.19**做GR/IR重分类 。GR/IR的借方余额调整成GIT，贷方余额调整成应付暂估,同时次月1日会自动产生冲销凭证。

**FI-MM业务集成:OBYC**

根据不同的采购业务场景，自动过账财务凭证

- BSX 存货记账

- PRD 成本差异(采购价差，生产订单差异。。)

- WRX GR/IR科目

- GBB 存货冲销(物料使用时的对方科目，如生产领料，销售发货时的对方科目）

  ![image-20240901174622803](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901174622803.png) 

- UMB ,PRA,PRY,FR1

评估修改：工厂的集群分组，工厂和科目表的连接标识

评估级别：物料类别

账户：会计科目

一般修改：移动动作

![image-20240901172142517](C:\Users\Rolin\AppData\Roaming\Typora\typora-user-images\image-20240901172142517.png)



