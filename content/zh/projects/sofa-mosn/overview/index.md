---
title: "SOFAMosn 介绍"
aliases: "/sofa-mosn/docs/Home"
---

[![Build Status](https://travis-ci.org/alipay/sofa-mosn.svg?branch=master)](https://travis-ci.org/alipay/sofa-mosn)
[![codecov](https://codecov.io/gh/alipay/sofa-mosn/branch/master/graph/badge.svg)](https://codecov.io/gh/alipay/sofa-mosn)
[![Go Report Card](https://goreportcard.com/badge/github.com/sofastack/sofa-mosn)](https://goreportcard.com/report/github.com/sofastack/sofa-mosn)
![license](https://img.shields.io/badge/license-Apache--2.0-green.svg)

SOFAMosn(Modular Observable Smart Network), 是一款采用 GoLang 开发的 Service Mesh 数据平面代理，旨在为服务提供分布式、模块化、可观察、智能化的代理能力。 SOFAMosn 通过 XDS API 与 SOFAMesh 集成，同时 SOFAMosn 可以作为独立的4、7层负载均衡使用，未来 SOFAMosn 将支持更多云原生场景，并支持 nginx 的核心转发功能。

## 核心能力

+ Istio集成
    + 集成 Istio 1.0 版本与 V4 API，可基于全动态资源配置运行
+ 核心转发
    + 自包含的网络服务器
    + 支持 TCP 代理
    + 支持 TProxy 模式
+ 多协议
    + 支持 HTTP/1.1，HTTP/2
    + 支持 SOFARPC
    + 支持 Dubbo 协议（开发中）
+ 核心路由
    + 支持 Virtual Host 路由
    + 支持 Headers/URL/Prefix 路由
    + 支持基于 Host Metadata 的 Subset 路由
    + 支持重试
+ 后端管理&负载均衡
    + 支持连接池
    + 支持熔断
    + 支持后端主动健康检查
    + 支持 Random/RR 等负载策略
    + 支持基于 Host Metadata 的 Subset 负载策略
+ 可观察性
    + 观察网络数据
    + 观察协议数据
+ TLS
    + 支持 HTTP/1.1 on TLS
    + 支持 HTTP/2.0 on TLS
    + 支持 SOFARPC on TLS
+ 进程管理
    + 支持平滑 reload
    + 支持平滑升级
+ 扩展能力
    + 支持自定义私有协议
    + 支持在 TCP IO 层，协议层面加入自定义扩展

## 快速开始

+ [参考这里](../quick-start-setup) 

## 社区

+ [Issues](https://github.com/sofastack/sofa-mosn/issues)

## 贡献

+ SOFAMosn 仍处在初级阶段，有很多能力需要补全，所以我们欢迎所有人参与进来与我们一起共建。

## 致谢

感谢 Google、IBM、Lyft 创建了 Envoy、Istio 体系，并开源了优秀的项目，使 SOFAMosn 有了非常好的参考，使我们能快速落地自己的想法。
