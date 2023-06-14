---
description: 工欲善其事，必先利其器
---

# 数据工具

本文总结我认为好用的量化数据工具，工具基本都使用python语言。本文只做系统性总结归纳，每个工具的具体用法，请参看各工具主页链接。

## 1. 数据获取

这是一切的源头，所以我们需要功能强大且稳定的数据获取工具。

### AKShare

> 主页：[https://akshare.xyz/](https://akshare.xyz/)

AKShare是目前我发现的最完善的开源、免费量化数据获取工具，作者水平在线，持续维护，更新速度快。其本质是网络爬虫，自己并不提供数据源。支持股票、指数、基金、债券、期货等全品类的数据接口。

优势：接口全网最丰富，源码质量高，更新维护快。

### pywencai

> 主页：[https://github.com/zsrl/pywencai](https://github.com/zsrl/pywencai)

pywencai是获取同花顺问财数据的开源python库，作者是我本人，它可以很方便的获取同花顺问财问句返回的数据。

优势：问财应用了AI技术，具备完善的自然语言处理能力，可以根据问句获取多种组合的数据。

### xtdata

> 主页：[http://docs.thinktrader.net/vip/pages/4a989a/](http://docs.thinktrader.net/vip/pages/4a989a/)

xtdata是miniQMT的一个模块，可以获取稳定的交易数据和财务数据，并具有行情实时订阅推送功能。

优势：具备稳定的数据源，数据粒度细，适合用作回测或实盘。

[《QMT开通规则分享》](https://i77j0z62us.feishu.cn/wiki/wikcnjb8jG8Aqt3aj6rM3JRMz2b)

## 2. 数据处理

获取回来的数据，很可能是很“脏”的，我们需要对数据进行清洗、处理。

### pandas

> 主页：[https://pandas.pydata.org/](https://pandas.pydata.org/)

pandas可以说是数据处理的必备技能，也是量化投资**必学**的技能，他可以很方便的处理一个数据序列或者一个数据表。

## 3. 数据存储

数据存储，有很多种方式，我个人的思路是，不需要追求过于复杂和精妙的存储方式，适合自己就行。

### csv（文件）

csv是最常见的一种二维数据表存储方式，可以使用pandas直接读取。

### json（文件）

json是web领域最常见的数据格式，量化领域，可以作为辅助配置文件，进行使用，不建议用它存储时序数据。

### HDF5（文件）

> 主页：[https://www.hdfgroup.org/solutions/hdf5/](https://www.hdfgroup.org/solutions/hdf5/)

HDF5是一种高性能数据存储文件格式，pandas原生支持。

### Feather（文件）

> 主页：[https://github.com/wesm/feather](https://github.com/wesm/feather)

Feather是[Apache Arrow](https://arrow.apache.org/)的静态数据存储格式，可以快速操作DataFrame数据，pandas原生支持。

### Parquet（文件）

> 主页：[https://parquet.apache.org/](https://parquet.apache.org/)

Apache Parquet 是一种开源的、面向列的数据文件格式，专为高效的数据存储和检索而设计。pandas原生支持。

### sqlite（文件型数据库）

> 主页：[https://www.sqlite.org/](https://www.sqlite.org/)

sqlite是文件，也是数据库，可以支持SOL查询，适合关系型数据的存储，python内置支持对sqlite的操作。

> 其他的数据库还有很多，比如mongoDB，mysql，influxedDB等，但这些数据库部署比较复杂，除非你要做很完善的数据系统，不然我认为没必要，会浪费很多时间，增加问题的复杂度。

###
