# 模式：客户端UI组成

## 问题

如何实现显示来自多个服务的数据的UI屏幕或页面？

## 解决方案

通过组成由多个[业务功能](https://microservices.io/patterns/cn/decomposition/decompose-by-business-capability.html)/特定于[子域的](https://microservices.io/patterns/cn/decomposition/decompose-by-subdomain.html)UI组件呈现的UI片段，在客户端上构建UI。

## 相关模式

- 所述[服务器端页面片段组成](https://microservices.io/patterns/cn/ui/server-side-page-fragment-composition.html)图案是一种替代方法