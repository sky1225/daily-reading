# Daily Reading

每天一篇英文技术文章。希望通过这个阅读计划可以提升大家与英文阅读能力与技术视野。

## 规则

* 要参加 Daily Reading 计划的同学可以添加微信「e7hanz」加入微信群。
* 群里每天发一篇技术文章，文章链接也会提交到 Github Repo 上。
* 群里的同学每周至少提交一篇笔记，否则需要在下一周的周一离开这个群，离开的同学也欢迎随时回来。
* 笔记不限于当周的文章，仓库里的任意一篇文章都可以。

## 提交笔记

* 在相应的目录下创建个人名字命名的文件即可，例如「xiaoming.md」。

## Index

## Distributed System
* 2020/11/03 - [Cache is the Root of All Evil](2020/11/3): 深入浅出的讨论了最基本的缓存一致性问题，比如读覆盖、写后读问题等。
* 2020/11/01 - [Strategies Used at Box to Protect MySQL at Scale](2020/11/1): Box 关于数据库访问层 (Data Access Layer) 的一些实践。
* 2020/11/04 - [Things I Learned to Become a Senior Software Engineer](2020/11/4): 当度过工作的第一年，发现简单的任务已经不再是挑战之后，如何在成为高级工程师的路上更进一步？Neil Kakkar 给出了他的一些思考。
* 2020/11/06 - [How We Learned to Stop Worrying and Read from Replicas](2020/11/6): 针对异步复制导致的主从不一致问题进行了讨论。
* 2020/11/09 - [Time, Clocks, and the Ordering of Events in a Distributed System](2020/11/9): 分布式领域必读 Paper。本文审视了在分布式系统中，一个事件发生在另一个事件之前的概念，并用它描述了事件的偏序关系。 给出了一种分布式算法，该算法用于同步逻辑时钟系统。
* 2020/11/14 - [Minimizing read-write MySQL downtime](2020/11/14): Yelp 的数据库高可用实践，分享怎么通过一个数据库代理中间层，实现多主切换的能力。
* 2020/11/18 - [The Google File System](2020/11/18): GFS，Google 的分布式文件存储系统。
* 2020/11/20 - [Cache coherency primer](2020/11/20): CPU 缓存一致性，详细的介绍了在多核、多缓存情况下如何确保 CPU 内的缓存一致性问题。和业务缓存的场景不一样，CPU Cache 是一个强一致性缓存。
* 2020/11/26 - [All things caching- use cases, benefits, strategies, choosing a caching technology, exploring some popular products](2020/11/26): 详细的介绍了缓存的适用场景、坑、收益，结合了从 CPU 到浏览器的各个层次缓存的实践分析。
* 2020/11/27 - [Edgar: Solving Mysteries Faster with Observability](2020/11/27): Netflix 的 APM 系统 Edgar，融合 Tracing、 Logging、Events，100% 采样，良好的场景化设计。
* 2020/11/29 - [Orchestrating Cassandra on Kubernetes with Operators](2020/11/29): Yelp 将它们的 Cassandra 集群从虚拟机平台（EC2）上迁移到了 Kubernetes 中，本文分享了这一迁移过程的实践。

## Architecture
* 2020/11/07 - [Building Airbnb's Internationalization Platform](2020/11/7): 讨论了 Airbnb 的国际化平台架构，这是一篇业务架构综述文章，对 i18n 领域的常见问题进行了介绍，以及讲解了 Airbnb 的实现方案。
* 2020/11/08 - [Architecting for Reliable Scalability](2020/11/8): 文章讨论了在对架构进行扩展时的一些常见实践，例如模块化、水平扩展、内容缓存等等。内容中有大量的 Reference，是一篇很好的领域综述性文章。
* 2020/11/11 - [Taming Service-Oriented Architecture Using A Data-Oriented Service Mesh](2020/11/11): Airbnb 的 Mesh 实践。不同于现在到处都在说的数据面、控制面等概念，Airbnb 一开始就以数据为中心来构建整个服务治理系统。
* 2020/11/12 - [Solid Relevance](2020/11/12): 距离 SOLID 原则提出已经过了 30 多年了，这个时间太久以至于不少人认为 SOLID 原则已经不再适用于现代软件工程。但 Uncle Bob 认为并不是这样的，软件工程的根基一直没有变化，SOLID 原则依然适用。在本文中 Bob 重新审视了 SOLID 五条原则在现代软件工程中的适用性。
* 2020/11/17 - [Building Software Systems At Google and Lessons Learned](2020/11/17): Jeff Dean 在 2010 年的分享，分享了 Google 从 1999 年到 2010 年间面临的各种不同的挑战，以及架构的演进。
* 2020/11/23 - [How LinkedIn scales compatibility testing](2020/11/23): LinkIn 有 12,000 个代码仓库，这些仓库之间有复杂的依赖关系。如何确保代码更新时对上下游的兼容性是可靠的？LinkIn 在这篇文章中分享了一些实践。
* 2020/11/24 - [On Designing and Deploying Internet-Scale Services](2020/11/24): 经典论文，讨论了设计一个后端系统时需要考虑的方方面面，例如面向故障设计、服务健康检查、底层组件零信任、版本管理、消除单点故障等等。架构师必读。

## Network
* 2020/10/29 - [A Trip Down the DNS Rabbit Hole: Understanding the Role of Kubernetes, Golang, libc, systemd](2020/10/29): 一次 Kubernetes 中 DNS 的故障排查过程。
* 2020/11/05 - [Keeping Netflix Reliable Using Prioritized Load Shedding](2020/11/5): 当请求变多，流量开始变得拥挤的时候，Netflix 通过给流量标记优先级实现了渐进式地流量降级。文章详细地讨论了该系统的设计、困难与实际效果。
* 2020/11/13 - [How Facebook is bringing QUIC to billions](2020/11/13): Facebook 的 QUIC 实践，包括 QUIC 的收益、推广过程、评估体系以及一些坑。

## Microservice
* 2020/10/30 - [Building Services at Airbnb, Part 4](2020/10/30): Airbnb 的微服务测试实践。
* 2020/11/16 - [Building Netflix's Distributed Tracing Infrastructure](2020/11/16): Netflix 的分布式链路追踪系统实践。

## Frontend
* 2020/10/28 - [When is no-code useful?](2020/10/28): 讨论了低代码平台存在的问题，以及作者认为低代码平台要解决的问题。文章中对于复杂度、软件工程的本质提出了一些看法。
* 2020/11/19 - [How We Build a Design System](2020/11/19): 如何构建一套设计系统。不仅仅介绍了设计系统是什么，还介绍了怎么运营这样一套设计系统。
* 2020/11/21 - [Micro Frontends Pattern Comparison](2020/11/21): 微前端框架是近几年比较热门的一个领域，本文讨论了几种常见的微前端框架范式。

## Career
* 2020/10/31 - [Engineering Onboarding Processes at Medium](2020/10/31): 了解 Medium 如何帮助新工程师融入环境。
* 2020/11/02 - [What do we need to know to start making a difference?](2020/11/2): 讨论了关于学习和实践的关系，作者将知识分为两类，分别讨论了如何获取这两类知识。
* 2020/11/10 - [Taking Ideas Seriously is Hard](2020/11/10): 讨论了「familiarity」与「taking sth seriously」的区别，比较有感触的是「复利」对于「学习」的影响。
* 2020/11/15 - [Making the most of your one-on-one with your manager or other leadership](2020/11/15): 一篇小短文，讲怎么提升 one-on-one 会议的效率。
* 2020/11/22 - [How do you write simple explanations without sounding condescending?](2020/11/22): 把复杂的事情讲简单是个强有力的能力，这篇文章给出了一些建议。
* 2020/11/25 - [Growth as a writer](2020/11/25): Linus Lee 作为一个非常高产的博主，提出了他认为的写作的三个阶段。
* 2020/11/28 - [Common Performance Review Biases: How to Spot and Counter Them](2020/11/28): 在绩效反馈中，我们并不总是可以收到清晰、公正的反馈，有些反馈会带有一些偏见。作者总结出了一些常见偏见模式，并且针对主管和成员都给出了很好的改正建议。
