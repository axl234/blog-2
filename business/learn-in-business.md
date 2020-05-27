# 前端在繁忙的业务中提升自己

> 我每天都在忙着写很多重复度高的业务，没有时间学习提升，感觉很焦虑怎么办？

> 我们的业务复杂度过低，对于自己技术提升没有帮助，要不要跳槽呢？

这个问题道中了许多程序员的心声，特别是刚毕业三年内几乎是被动接受领导分配任务的同学们。那山月来总结梳理一下如何脱身于复杂的业务逻辑，并提升自己

## 解决痛点问题

在一个产品的生命周期中必然会伴随着众多的问题，前端在解决问题中也贡献着自己的一份力，并为应用的稳定保驾护航。比如作为前端而言，必然要解决以下问题:

1. 网站打开速度过慢
1. 网站部署速度过慢
1. 线上反馈问题过多

这三个问题无论哪一个都过于宏大，无论哪一个被解决掉都对技术提升有很大帮助，而且能够在简历和绩效考核上添加浓墨重彩的一笔。等你深入职场几年，你就能够知道大厂面试中最重要的不是理论知识，而是你在

对于第一个问题：网站打开速度过慢。仔细一瞧，这不是那个前端面试必背的面试题吗: 如何优化网站的性能？这样你对它不仅有了理论知识，也有了实践经验，在面试官咄咄逼问下也能对答如流。

对于第二个问题：网站部署速度过慢。你在解决这个问题的心路历程可能是这样子的 (毕竟我在解决这个问题的心路历程是这样子的)

1. 我家这个网站是如何部署的？要解决部署问题，首先得知道它是如何部署的
    1. 页面资源(html)是否与静态资源(js/css)分离？
    1. 静态资源是否上了 CDN？
    1. CDN 提供商是哪一家，它家的 CDN 怎么配置？
    1. 静态资源上了 CDN 要注意什么问题？为什么有一次用户反馈只有他们的页面打不开？为什么有一次新版本部署上去但未生效？
    1. 静态资源上传 CDN 时，如何提高上传速度，以此来提高网站的部署速度
    1. CDN 回源过多，命中率过低怎么解决？
1. 打包体积终于被我弄小了，依赖安装及打包的时间又过长，那我应该如何优化呢 (又延伸出 CI，webpack 及 npm 若干问题)
    1. 安装依赖是否有更有效更快地方法呢？
    1. 打包是在 CI 下打包的？CI 又是什么
    1. CI 下如何利用缓存，避免每次都要安装依赖？
    1. 如何优化 webpack 打包的时间，原理都是什么
    1. 当 webpack 利用多进程多线程打包优化时，我的 CI 有几个 CPU 核心，这一点是否有所帮助
    1. 即使 CI 的核心数很多，如果有并行的多个流水线，CI 的 cpu 会不会爆掉

这其中涉及到了大部分前端都不会接触的技术与能力，这对自己的项目实战能力以及工程化能力都有大幅提高。比如

1. 操作系统，特别是其中涉及到的进程与线程，文件系统甚至是 CPU 在部署优化时扮演重要角色
1. DevOps，如 CI 中的部署优化，甚至可能有最近大火的容器与 docker
1. CDN，了解网站部署到 CDN 的过程及可能出现的问题
1. webpack

> 你以为面试官总喜欢问基础问题吗，不，他们更喜欢问在项目实战中的成就感及重难点。

## 解决用户反馈

最直观，最紧急，最亟待解决的问题就是异常监控系统上的报警与用户反馈，毕竟他们与生产环境相关，与用户相关。如果说以上痛点问题已被其它同学大包大揽了，被他们预定了 KPI/OKR，提前写到了简历及 PPT 上。那解决用户的反馈绝对是一个可以够得着，让他人看得见并提高自己的一个渠道。况且解决问题与需求开发是整个产品开发中最重要的两个问题。

比如在一个 toB 产品中，多个用户提出了某特定功能不可用的反馈。

经排查，是浏览器兼容性问题，此时，作为一个 toB 产品，你可以回馈用户，换个谷歌浏览器。但更好的方式是对于不兼容浏览器，提示用户需要使用最新的浏览器方式打开。一个简单又不复杂的技术实现，却有着更高的收益。

线上问题多种多样，有的繁琐，有的复杂，但无一不提高你解决问题的能力。反馈处理多了，必将形成新的抽象与思考

1. 如何快速定位问题，这将涉及到异常上报，线上调试，业务能力，技术水平等综合能力
1. 快速上线后用户多久可见正确效果，这将涉及到 Git 工作流以及CI 工作流。(五分钟能改好吗？不能，光上线就得五分钟。)

## 提升业务能力

技术与业务紧紧相关，什么样的业务就有什么样的技术，对业务的了解深入也相应促进对技术的深入。