# yurun-crawler

yurun-crawler 是一个分布式高性能爬虫采集框架，基于 imi + Swoole 协程的常驻内存开发。

> 分布式，高性能，一把梭！

## 概念

### 下载器

负责请求网址，下载并存储内容。

多协程的架构下，支持同时下载海量数据。

### 数据模型

定义需要从页面中，提取的内容属性。

### 解析器

负责解析下载后的内容，从中提取需要的信息。

首个版本支持：Dom 解析、正则、JSON。

### 存储器

将解析后的数据存储入库。

### 触发器

支持监听各环节事件，以便做个性化处理。

### 代理 IP 池

实现代理 IP 池抽象，开发者可以很方便地对接不同接口方。
