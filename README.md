# kratos 初体验

## 项目简介
1.kratos（来自于希腊战神 奎托斯）

2.kratos 是 bilibili 一套Go微服务开发框架及工具

3.源码：https://github.com/bilibili/kratos


## 微服务特性
1.高内聚，低耦合；服务独立测试、部署、升级、发布；运行在独立的进程

2.服务与服务之间 轻量级的通信机制

3.按业务需求定制服务，选择不同的技术栈。

## 使用

##### Requirments

Go version>=1.12 and GO111MODULE=on

##### Installation

下载框架

go get -u github.com/bilibili/kratos/tool/kratos

cd $GOPATH/src

生成基于kratos库的脚手架代码,同时生成通过 protobuf 定义的grpc和bm示例代码	

kratos new kratos-demo -o serenity --proto


##### Build & Run
cd $GOPATH/src/kratos-demo/cmd

go build

./cmd -conf ../configs

