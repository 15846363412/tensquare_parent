# tensquare_parent
第一天练习
学习devops相关概念、工具链、行业标准

一、devops相关概念：

		DevOps一词来自于Development和Operations的组合，突出重视软件开发人员和运维人员的沟通合作（开发和部署），是一组过程、方法与系统的统称，促进开发rd与技术运营和质量保证qa之间的沟通、协作和整合。

		DevOps是一种方法或理念，它涵盖开发、测试、运维的整个过程。DevOps是提高软件开发、测试、运维、运营 等各部门的沟通与协作质量的方法和过程，DevOps强调软件开发人员与软件测试、软件运维、质量保障（QA）部 门之间有效的沟通与协作，强调通过自动化的方法去管理软件变更、软件集成，使软件从构建到测试、发布更加快 捷、可靠，最终按时交付软件。简单说就是开发运维一体化

 dev：                                      ops:

code -> buid ->test->release->deploy->operate->monitor->plan->code

相关术语

		产品迭代：在现实工作中，往往都是用户不知道自己想要什么，但是当我们设计完一个产品后，他后告诉我们不需要什么，这样我们的产品需要反复的迭代

       技术革新：技术架构随着系统的负责化不断的更新。

		敏捷开发：敏捷开发(Agile Development)是一种以人为核心、迭代、循序渐进的开发方法（小的需求快速发布上线）。具体方式：scrum和xp。

		持续集成 （Continuous integration，简称CI）：持续集成是指不断整合项目更改并进行相应的测试

作用：代码库存越是积压，就越得不到生产检验，积压越多，代码间交叉感染的概率越大，下个发布（release）的复杂度和风险越高，持续集成可以保证团队开发人员提交代码的质量，减轻了软件发布时的压力；持续集成中的任何一个环节都是自动完成的，无需太多的人工干预，有利于减少重复过程以节省时间、费用和工作量；及早的发现代码中的问题，及早解决，代码越早推送（PUSH）出去，用户能越早用到，快就是商业价值；

        持续交付（Continuous delivery）：

        持续部署CD：

				

二、工具链

DevOps兴起于2009年，近年来由于云计算、互联网的发展，促进了DevOps的基础设施及工具链的发展，涌现了 

一大批优秀的工具，这些工具包括开发、测试、运维的各各领域，例如：GitHub、Git/SVN、Docker、Jenkins、 Hudson、Ant/Maven/Gradle、Selenium、QUnit、JMeter等。下图是DevOps相关的工具集：







1.Git:分布式版本控制系统



个人电脑上安装Git，过程略。 

注意：Git安装完成需配置user.name和user.email

2.GitLab：是一个git的企业级远程代码仓库，类似的还有码云gitee，github

查询user.name和uesr.email 

    git config user.name 
    
    git config user.email 
    
    设置： 
    
    git config ‐‐global user.name "zhuyongliang" 
    
    git config ‐‐global user.email "zhuyongliang@ebupt.com" 

gitlab的界面



3.Docker：一个开源的应用容器引擎，让开发者可以打包他们的应用以及依赖包到一个可移植的容器中，然后发布到 linux上，也可以实现虚拟化。容器是使用沙箱机制，相互之间不会有任何接口。docker是基于go语言开发的

官网：：https://www.docker.com/ 

虚拟化技术相当于虚拟出一个小型的计算机，他是依赖于宿主机linux系统的。为了有效利用计算机资源，开箱即用。



docker安装：

    在centos7上直接通过yum命令：
    
    					yum install -y docker 
    
    					启动docker：service docker start 
    
    					查询docker版本:docker version 

jenkins：Jenkins是一个领先的开源自动化服务器，可用于自动化构建，测试，部署软件等相关任务。



---



三、行业标准

术语：

		配置项  configuration item

		制品 artifact

		代码复杂度 code complexity

		部署流水线 deployment pipeline

持续交付：持续交付是指持续的将各类变更（包括新功能、缺陷修复、配置变化、实验等）安全、快速、高质
量地落实到生产环境或用户手中的能力



1. 配置管理       版本控制   变更管理
2. 构建与持续集成
3. 测试管理
4. 部署与发布管理
5. 环境管理
6. 数据管理
7. 度量和反馈

技术要求表：




