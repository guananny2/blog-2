# 前端在繁忙的业务中提升自己 (约稿)

> 我每天都在忙着写很多重复度高的业务，没有时间学习提升，感觉很焦虑怎么办？

> 我们的业务复杂度过低，对于自己技术提升没有帮助，要不要跳槽呢？

这个问题道中了许多程序员的心声，特别是刚毕业三年内几乎是被动接受领导分配任务的同学们。那山月来总结梳理一下如何脱身于复杂的业务逻辑，并提升自己

## 解决痛点问题

在一个产品的生命周期中必然会伴随着众多的问题，前端在解决问题中也贡献着自己的一份力，并为应用的稳定保驾护航。比如作为前端而言，必然要解决以下问题:

1. 网站打开速度过慢
1. 网站部署速度过慢
1. 线上反馈问题过多

这三个问题无论哪一个都过于宏大，无论哪一个被解决掉都对技术提升有很大帮助，而且能够在简历和绩效考核上添加浓墨重彩的一笔。

**等你深入职场几年，在大厂面试中你就能够知道最重要的不是理论知识，而是你在实际工作中解决了哪些棘手的问题**

对于第一个问题：网站打开速度过慢。仔细一瞧，这不是那个前端面试必背的面试题吗: 如何优化网站的性能？这样你对它不仅有了理论知识，也有了实践经验，在面试官咄咄逼问下也能对答如流。

对于第二个问题：网站部署速度过慢。你在解决这个问题的心路历程可能是这样子的

1. 我家这个网站是如何部署的？要解决部署问题，首先得知道它是如何部署的
    1. 页面资源(html)是否与静态资源(js/css)分离？
    1. 静态资源是否上了 CDN？
    1. 静态资源上了 CDN 要注意什么问题？为什么有一次用户反馈只有他们的页面打不开？为什么有一次新版本部署上去但未生效？
    1. 静态资源上传 CDN 时，如何提高上传速度，以此来提高网站的部署速度
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

线上问题多种多样，有的繁琐，有的复杂，但无一不提高你解决问题的能力。反馈处理多了，必将形成新的抽象与思考

1. 如何快速定位问题，这将涉及到异常上报，线上调试，业务能力，技术水平等综合能力
1. 快速上线后用户多久可见正确效果，这将涉及到 Git 工作流以及CI 工作流。(五分钟能改好吗？不能，光上线就得五分钟。)

## 小结

在复杂的业务逻辑这个大工程中，你只有拥有足够大能够 hold 住整个业务的大工程化能力，你才能脱身于业务，并站在更高点来思考与理解业务。这种核心工程能力包括异常系统建设及监控，部署时的持续集成，还有打包上线过程中会遇到的各种问题。

而这种实战性的能力又很难通过自学来获得，这里送出一套网易云课程的前端进阶直播课

网易【网易高级前端开发系列第③期直播课】晚上8点准时发车哦🚄
赶快搬好小板凳呀

+ 🍭【技能】：3月28日：手把手带你用node构建中间层
+ 🍭【技能】：3月30日：晋升前端负责人必修课-如何构建前端标准
+ 🍭【架构】：3月10日：打通全栈，轻松掌握服务端渲染
+ 🍭【技能】：3月11日：程序员的真正能力-代码质量如何提高
+ 🍭【技能】：3月11日：程序员的真正能力-以系统系统建设

戳此加入直播课程学习，上课前会有提醒哦：https://study.163.com/sl/4pB，晚8点直播准时开始，记得提前进入直播间占位置哦~

在大厂中，这些核心工程能力会进一步提炼与抽象，形成大厂独有的前端技术基建能力，这里有一份关于网易，阿里等互联网大厂关于前端基建实践的资料可供下载：
