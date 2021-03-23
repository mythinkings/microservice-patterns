# 模式：命令查询责任隔离（CQRS）

## 问题

如何在微服务架构中实现查询

## 解决方案

将应用程序分为两部分：命令端和查询端。命令端处理创建，更新和删除请求，并在数据更改时发出事件。查询端通过对一个或多个实例化视图执行查询来处理查询，这些实例化视图通过订阅数据更改时发出的事件流来保持最新。

## 相关模式

- “[每个服务](https://microservices.io/patterns/cn/data/database-per-service.html)的[数据库”模式](https://microservices.io/patterns/cn/data/database-per-service.html)创建了对此模式的需求
- 在[事件驱动的架构](https://microservices.io/patterns/cn/data/event-driven-architecture.html)图案生成事件流
- 该[事件的采购](https://microservices.io/patterns/cn/data/event-sourcing.html)通常与CQRS使用

## 例子

- 请参阅使用事件源和CQRS的[Eventuate示例应用程序](http://eventuate.io/exampleapps.html)。