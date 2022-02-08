# Heroku-vless

再次声明，免费服务，且用且珍惜，尽量不要滥用。

## 简介
Heroku是一个支持多种编程语言的云平台即服务。目前支持Ruby、Java、Node.js、Scala、Clojure、Python、PHP和Perl等语言，基础操作系统是Debian。

本项目用于在 Heroku 上部署 vless+websocket+tls，每次部署自动选择最新的 alpine linux 和 xray core。相比vmess，vless的性能更加优秀，占用资源更少，运行更加稳定。

建议使用cloudflare的workers的流量中转，速度更快，原则上使用后不会有被墙风险。

## 一键部署

经测试本镜像占用内存资源较低，运行稳定。点击下方紫色图标部署。

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://dashboard.heroku.com/new?template=https%3A%2F%2Fgithub.com%2Frptec%2Fheroku-vless)


#### 注：失效问题
上方一键部署已失效，刚看到有朋友说heroku检测到代码违反服务协议，估计使用的人太多或被人举报仓库被heroku封了。

#### 解决方法：
a.这里建议你fork本代码后，在github里设置为私有，然后绑定你github到heroku部署使用，推荐这个。

b.或者也可以fork代码后，修改下面链接rptec为你自己账户名，通过链接部署。

https://dashboard.heroku.com/new?template=https://github.com/rptec/heroku-vless.git

