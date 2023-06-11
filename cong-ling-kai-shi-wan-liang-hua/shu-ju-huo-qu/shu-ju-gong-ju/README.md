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

### pandas

## 3. 数据存储
