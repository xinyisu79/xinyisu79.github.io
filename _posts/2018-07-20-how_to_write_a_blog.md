---
layout: post
title: Blogging Like a Hacker
categories: post
---

# HBase源码阅读
## HBase概述
HBase是一种专门为半结构化数据和水平扩展性设计的数据库。它把数据存储在表中，表按“行健(row key)，列簇(Column Family)，列限定符(Qualifier)和时间版本(timestamp)”的四维坐标系来组织。HBase是无模式数据库，只需要提前定义列簇，并不需要指定列限定符。同时它也是无类型数据库，所有数据都是按二进制字节方式存储的，对HBase的操作和访问有5个基本方式，即 Get、Put、Delete 和 Scan 以及 Increment。HBase 基于非行健值查询的唯一途径是通过带过滤器的扫描。
