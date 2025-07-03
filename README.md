# LearningArch

## AWS

- IAM
  - [IAM Policy](https://security.kpingfan.com/01.iam/1.concepts/)
  - [STS Token](https://security.kpingfan.com/01.iam/2.practices/)
  - [Role Anywhere](https://security.kpingfan.com/01.iam/3.iam-role-anywhere/)
  - [IAM Identity Center](https://security.kpingfan.com/01.iam/5.iam-ientity-center/)
  - [AWS IAM Anywhere 使用 X.509 數位憑證交換 IAM Role session token](https://shazi.info/aws-iam-anywhere-%e4%bd%bf%e7%94%a8-x-509-%e6%95%b8%e4%bd%8d%e6%86%91%e8%ad%89%e4%ba%a4%e6%8f%9b-iam-role-session-token/)
  - [AWS的无AK实践](https://blog.chengchao.name/2024/03/20/aws-temporary-credentials/)

## Linux

  - 多路复用IO
    - [epoll原理剖析#1： I/O与等待队列](https://medium.com/@heshaobo2012/epoll%E5%8E%9F%E7%90%86%E5%89%96%E6%9E%90-1-i-o-d062d47fb07a)
    - [epoll原理剖析#2： select & poll](https://medium.com/@heshaobo2012/epoll%E5%8E%9F%E7%90%86%E5%89%96%E6%9E%90-3-select-poll-8d23b0a12906)
    - [epoll原理剖析#3： epoll](https://medium.com/@heshaobo2012/epoll%E5%8E%9F%E7%90%86%E5%89%96%E6%9E%90-3-epoll-bf9cdcf5e50)
  - Capabilities
    - [Linux Capabilities 入门教程：概念篇](https://fuckcloudnative.io/posts/linux-capabilities-why-they-exist-and-how-they-work/)
  - Cgroup
    - [Linux资源管理之cgroups简介](https://tech.meituan.com/2015/03/31/cgroups.html)
  - Linux 命令
    - [Linux 命令搜索引擎](https://wangchujiang.com/linux-command/)
## 云原生

  - istio
    - [官方文档](https://istio.io/latest/zh/docs/)
    - [Istio中文教程](https://www.orchome.com/istio/index)
    - [云原生之容器安全实践](https://tech.meituan.com/2020/03/12/cloud-native-security.html)：还没看，有空看看
   
### 容器

- Docker
  - [Docker 从入门到实践](https://yeasy.gitbook.io/docker_practice/) 

### 编排系统

- Kubernetes
  - [kubernetes-handbook](https://jimmysong.io/kubernetes-handbook/)
  - [kubernetes官方文档](https://kubernetes.io/zh/) 
  - [和我一步步部署 kubernetes 集群](https://k8s-install.opsnull.com/)
 
## 中间件

- **key-value存储**
  - etcd
    - [etcd官方文档中文版](https://doczhcn.gitbook.io/etcd/index)
    - [raft一致性算法动画演示](http://thesecretlivesofdata.com/raft/)
    - [Etcd 架构与实现解析](http://jolestar.com/etcd-architecture/)
- **代理**
  - Nginx
    - [Nginx 极简教程](https://dunwu.github.io/nginx-tutorial/#/nginx-quickstart)
    - [Nginx 中文文档](https://www.docs4dev.com/docs/zh/nginx/current/reference)
    - [agentzh 的 Nginx 教程](https://openresty.org/download/agentzh-nginx-tutorials-zhcn.html)
    - [Nginx 配置自动生成](https://www.digitalocean.com/community/tools/nginx?global.app.lang=zhCN)
  - Apache Httpd
    - [Apache 教程](https://www.yiibai.com/apache_http)
    - [Apache HTTP 服务器 2.4 文档](http://httpd.apache.org/docs/2.4/)
  - APISIX
    - [apisix 快速入门指南](https://apisix.apache.org/zh/docs/apisix/getting-started/)
    - [APISIX架构分析：如何动态管理Nginx集群？](https://mp.weixin.qq.com/s/DtCyZkFzNKnRBaMnGcUx1Q)
- **监控**
  - prometheus
    - [Prometheus操作指南](https://yunlzheng.gitbook.io/prometheus-book/)
    - [Prometheus官方文档中文版](https://sheldon-lu.github.io/sheldon_Gitbook/)
- **消息中间件**
  - kafka
    - [kafka官方文档](https://kafka.apache.org/documentation/)
    - [kafka中文教程](https://www.orchome.com/kafka/index)
    - [Kafka理论之Consumer Group & Coordinator](https://yhyr.github.io/2018/12/26/Kafka%E7%90%86%E8%AE%BA%E4%B9%8BConsumer-Group-Coordinator/)
    - [Kafka消费者组再均衡问题](https://www.cnblogs.com/FG123/p/10095125.html)
    - [Configurable SASL callback handlers](https://cwiki.apache.org/confluence/display/KAFKA/KIP-86%3A+Configurable+SASL+callback+handlers)
  - pulsar
    - [pulsar 中文文档](https://pulsar.apache.org/docs/zh-CN/standalone/)
   
## 安全设计

- 认证鉴权
  - [认证鉴权相关的概念](https://docs.authing.cn/v2/concepts/federation.html)    
  - [基于PBAC模型构建零信任IAM平台](https://mp.weixin.qq.com/s/OdDfwK7afKzRgX280FgDTg)
  - [浅谈零信任之访问控制模型](https://www.freebuf.com/articles/network/279497.html)
  - kerberos
    - [Kerberos-维基百科](https://zh.wikipedia.org/wiki/Kerberos)
    - [KERBEROS PROTOCOL TUTORIAL](https://www.kerberos.org/software/tutorial.html)
  - LDAP
    - [LDAP系列（1）：快速搭建 LDAP 服务器](http://guleilab.com/2018/07/24/LDAP1/)
  - OAuth2
    - 阮一峰OAuth系列教程
      - [1. OAuth 2.0 的一个简单解释](http://www.ruanyifeng.com/blog/2019/04/oauth_design.html)
      - [2. OAuth 2.0 的四种方式](http://www.ruanyifeng.com/blog/2019/04/oauth-grant-types.html)
      - [3. GitHub OAuth 第三方登录示例教程](https://www.ruanyifeng.com/blog/2019/04/github-oauth.html)
    - [『OAuth2.0』 猴子都能懂的图解](https://learnku.com/articles/20031)
  - SSO
    - [SSO单点登录看这一篇就够了](https://github.com/Snailclimb/JavaGuide/blob/master/docs/system-design/authority-certification/SSO%E5%8D%95%E7%82%B9%E7%99%BB%E5%BD%95%E7%9C%8B%E8%BF%99%E4%B8%80%E7%AF%87%E5%B0%B1%E5%A4%9F%E4%BA%86.md)
- 证书
  - [CA认证和颁发吊销证书](https://www.cnblogs.com/along21/p/7595912.html)

## Misc

- Git
  - [廖雪峰的git教程](https://www.liaoxuefeng.com/wiki/896043488029600)
  - [猴子都能懂的git入门](https://backlog.com/git-tutorial/cn/intro/intro1_1.html)
- base64
  - [Base64笔记](http://www.ruanyifeng.com/blog/2008/06/base64.html)
