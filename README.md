<h1 align=center>研发报告<h1>

## 目录  
  
  * 引言  ---------------------------------------------------------------------------------------------------------------------- 2  
  
    * 编写目的  ------------------------------------------------------------------------------------------------------------ 2  
    
    * 背景  ----------------------------------------------------------------------------------------------------------------- 2  
    
    * 专业术语  ------------------------------------------------------------------------------------------------------------ 3  
    
    * 参考资料  ------------------------------------------------------------------------------------------------------------ 3  

  * 项目研发过程  ------------------------------------------------------------------------------------------------------------ 3

    * 需求分析  ------------------------------------------------------------------------------------------------------------ 3

    * UI & API 设计  ------------------------------------------------------------------------------------------------------- 3

    * 编码 & 测试  --------------------------------------------------------------------------------------------------------- 3

    * 上线维护  ------------------------------------------------------------------------------------------------------------ 3


  * 需求分析  ----------------------------------------------------------------------------------------------------------------- 3  
  
    * 整体介绍  ------------------------------------------------------------------------------------------------------------ 3  
    
    * 参与方  --------------------------------------------------------------------------------------------------------------- 3  
    
    * 用户  ----------------------------------------------------------------------------------------------------------------- 3  
    
    * 工作室  --------------------------------------------------------------------------------------------------------------- 4  
    
    * 要求  ----------------------------------------------------------------------------------------------------------------- 4  


  * 项目组及成员分工安排  -------------------------------------------------------------------------------------------------- 4  

    * 前端：李聪、满磊、路萍  ------------------------------------------------------------------------------------------- 4  

    * 后端：冯伟赞、朱修羽  ---------------------------------------------------------------------------------------------- 4  

    * 文档：全体成员  ------------------------------------------------------------------------------------------------------ 4  

  * 需求变化 & 变更  ---------------------------------------------------------------------------------------------------------- 4

    * 时间  ------------------------------------------------------------------------------------------------------------------ 5

    * 应对策略  ------------------------------------------------------------------------------------------------------------- 5

  * 软件设计  ------------------------------------------------------------------------------------------------------------------ 5  
  
  * 关键技术  ------------------------------------------------------------------------------------------------------------------ 5  

  * 辅助工具  ------------------------------------------------------------------------------------------------------------------ 5  

    * 协同开发  ------------------------------------------------------------------------------------------------------------- 5  

    * 设计  ------------------------------------------------------------------------------------------------------------------ 5  

    * 前端  ------------------------------------------------------------------------------------------------------------------ 5  

    * 后端  ------------------------------------------------------------------------------------------------------------------ 5  

  * 统计数据  ------------------------------------------------------------------------------------------------------------------ 5  

    * 需求功能点  ----------------------------------------------------------------------------------------------------------- 5  

    * 文档规模数  ----------------------------------------------------------------------------------------------------------- 5  

    * 代码行  ------------------------------------------------------------------------------------------------------------------ 6  


  * 测试  ------------------------------------------------------------------------------------------------------------------ 6  
  
  * 验收标准  -------------------------------------------------------------------------------------------------------------- 6  
  
    * 项目验收需要提交的内容----------------------------------------------------------------------------------------- 6  
      *  最终系统  ---------------------------------------------------------------------------------------------------- 6  

      * 可运行的系统demo  ------------------------------------------------------------------------------------------ 6  

      * 源代码  ------------------------------------------------------------------------------------------------------- 6  

      * 必须提交的文档制品  ---------------------------------------------------------------------------------------- 6  
    * 验收报告  ---------------------------------------------------------------------------------------------------------- 6  
    
      * 项目报告  ----------------------------------------------------------------------------------------------------- 6  
      
      * 个人报告  ----------------------------------------------------------------------------------------------------- 7  
      
    * 系统和能力演示  -------------------------------------------------------------------------------------------------- 7  
    
      * 项目演示和个人演示  ---------------------------------------------------------------------------------------- 7  
      
      * 项目演示  ---------------------------------------------------------------------------------------------------- 7  
      
      * 个人工具使用  ------------------------------------------------------------------------------------------------ 7  
      
      * 个人项目成果展示  ------------------------------------------------------------------------------------------- 7  
      
      
## 引言
* 编写目的
  >为了SchoolInApp在开发和维护过程中使用的。在开发过程中，当开发人员有疑惑时，可以查询本文档，明确SchoolInApp的需求；可以清楚的查看SchoolInApp的设计过程，明确需要需要完成的功能；查看测试环节，明确SchoolInApp是如何测试的；查看验收标准，了解SchoolInApp的质量情况。

* 背景
  * 软件名称  
  >软件名称为：ScholInApp
  * 任务提出者  
  >南京大学计算机系张天老师作为项目的发起人，项目需求来源于实验课程，由张天老师扮演项目发起人，提出用户需求。
  * 开发者
  >在葛笑飞同学的指导下，由李聪，冯伟赞，满磊，陆萍，朱修宇五位大三同学组成的开发团队，共同完成整个项目的开发,其中李聪作为team leader。
  * 用户
  >SchoolInApp的使用用户分为两类，包括所有南京大学的本科生以及老师。注册用户时需要使用南京大学邮箱，非南京大学人员没有权限使用SchoolInApp。

* 专业术语
  * SchoolInApp：软件的名称  
  
  * studio:工作室  
  
  * essay:工作室发的文章  
  
  * question: 用户或者工作室提出的问题  
  
  * REST: Representational state transfer  
  
  * API: Application Programming Interface  
  
  * spring: 应用程序框架  
  
* 参考资料
  * [客户端开发平台](https://developer.android.com/index.html)
  * [服务器端开发平台](https://spring.io/)  
  * [Android开发规范](http://www.androidchina.net/2141.html)  
  * [后端java开发规范](http://www.hawstein.com/posts/google-java-style.html)  
  * [开发者单位](https://cs.nju.edu.cn/)  
  * [REST](https://en.wikipedia.org/wiki/Representational_state_transfer)
  * [spring](https://en.wikipedia.org/wiki/Spring_Framework)
  * [API](https://en.wikipedia.org/wiki/Application_programming_interface)


##  项目研发过过程

  * 需求分析  

  * UI & API 设计  

  * 编码 & 测试  

    * 基于文本的App（60%）  

    * Https/Cookie和通知机制（5%）  

    * 基于富文本的App（25%）  

    * 语音功能（5%）  

    * 界面调整与优化（5%）

  * 上线 & 维护  


## 需求分析  

* 整体介绍
  * 该App是一个以`兴趣`和`问题`驱动的知识咨询共享服务平台。
* 参与方
  * 该App由`个人用户`和`工作室成员`参与互动，从而让工作室可以为个人用户提供知识咨询和共享服务。

* 用户  

  * 注册进入该App的用户为南大在校校职工，凭南大个人邮箱进行注册。注册后的用户可以:  
    
    * 浏览热门问题/文章，并对问题/文章进行点赞，对文章进行评论。  
    
    * 向某个工作室咨询问题。  
    
    * 通过资历证明材料，提出组建工作室的申请，并在通过后组建工作室，从而对外提供知识咨询和共享服务。  
    
* 工作室  

  * 工作室的成员可以：  
  
    * 为个人用户做出解答。  
  
  * 工作室管理员可以发表文章进行知识共享。  
  
* 要求  

  * 工作室必须由运营团队建立，工作室人数上限10个人。  
  
  * 采用实名制，凭学校邮箱发验证码进行注册。  
  
  * 用户提问可以用文字图片。但只能对工作室进行提问。  
  
  * 工作室人员回答用户问题可以用文字图片语音。同一成员可以多次回答同一问题，但回答后只可删除不可以修改。  
  
  * 工作室(管理员)可以以主题的方式发布一篇文章，形式可以为文字、图片、语音，但必须有文字。  
  
  * 用户可以对文章进行评论，可以多次评论同一文章，但评论后只可删除不可以修改；评论必须实名，不可匿名；评论只能用文字和图片；文字需要检查污言秽语；允许别人举报其他人的评论；不需要链状评论；  
  
  * 用户发的问题在有答案之前可以自己删除，但有答案后问题的删除权限交给工作室。  
  
  * 用户可以对文章或问题点赞，但点赞只能针对文章或问题。用户点赞的历史可以看得到。  
  
  * 工作室可以对问题/文章的评论进行加精或者置顶。  
  
  * 用户可以收藏。  
  
  * 问题相似度检索推荐。  
  
  * 首页有问题推荐。  


## 项目组及成员分工安排
  
  * 前端：李聪、满磊、路萍  
    * 李聪：登录注册页面；个人信息页面(包括好多个子页面，收藏、已提问收藏回答问题等)；团队信息页面；  

    * 满磊：提问(定向、不定向)页面；写文章页面；搜索页面；  

    * 路萍：文章展示页面，包括对文章的评论展示页面；问题页面，包括对问题的评论展示页面；回答展示页面，包括对回答的评论展示页面；  

  * 后端：冯伟赞、朱修羽  

    * 冯伟赞：用户、问题、回答；搜索；富文本；语音  

    * 朱修羽：工作室、文章、评论；通知机制  

  * 文档：全体成员  

    * 路萍、朱修羽：需求文档、设计文档、demo录制  

    * 满磊：工作日志、研发报告、用户手册  

    * 冯伟赞：后端测试计划、后端测试报告、前后端测试报告和计划的整合  

    * 李聪：前端测试计划、前端测试报告、项目报告  
    
## 需求变化&变更  

  * 需求发生变更  

    * 时间  
      
      * 我们组正处于API设计完成阶段

    * 应对策略  

      *   校园问答集体需求讨论  

      * 确定会议召开后  

      * 由于相对于我们本来的设计的需求和API来说有所缩小，因此我们也将API缩小  

      * 放到dev分支下，原API在master分支下  
      
## 软件设计  
详情见设计报告  

## 关键技术  
  
  * 贯穿：git  

  * 设计：PhotoShop，Schetch，RESTful，HTTP  

  * 基于文本的 App ：android 基础，tomcat/spring/hibernate 基础  

  * 通知机制：实现原理  

  * 基于文本的安全 App ：HTTPS/SSL/TSL，IP-Based-Self-Signed-Certificate  

  * 基于富文本的 App ：Glide，HTTP Multipart，Apache Lucene  

  * 基于语音的 App ：android 存储  

## 辅助工具  
  
  * 协同开发：git  

  * 设计：PhotoShop，Schetch  

  * 前端：

    * 开发工具：Android Studio 3.1  

    * 辅助类库： Gson; CircleImageView; Glide; ButterKnife; Okhttp3; Retrofit; Otto; BRVAH; JPush; RichEditor; FloatingActionButton; Espresso;  

  * 后端：  

    * 开发工具：IntelliJ IDEA  

    * 辅助类库：spirngframework; commone-fileupload; hibernate; jackson; log4j; jsoup; lucene  

## 统计数据  
  
  * 需求功能点：16（详见需求文档）  

  * 文档规模数  

    * 需求文档：15页  

    * 设计文档  

  * 代码行： $ find . -name "*.java" | xargs cat | grep -v ^$ | wc -l   

    * 前端：15k +  

    * 后端：9k +  

## 测试
详情见测试报告

## 验收标准

一、项目验收需要提交内容（按顺序形成文件目录）：  

  * 最终系统：  
    
    * 安装包：将系统打包成一键安装包，自含各类支撑软件（插件、中间件、数据库等）；有APP、客户端、服务器端，则分别打包；  
      
    * 安装说明：说明安装包中文件用途；  
    
  * 可运行的系统demo：  
    
    * 使用录屏软件准备一个带语音讲解的demo视频，不超过15分钟，展示从安装、主要功能要点的使用；  
    
  * 源代码：  
    
    * 源代码  
    
    * 代码说明文档，按文件组织结构介绍系统的构成和各文件的用途  
    
  * 必须提交的文档制品：  
    
    * 需求分析说明书  
    
    * 设计说明书  
    
    * 分析和测试计划  
    
    * 分析和测试报告  
    
    * 用户手册  
    
    * 项目研发报告   
    
    * 工作日志  
    
    
二、验收报告：验收报告分项目报告和个人报告两个部分，准备ppt，项目组长介绍项目、成员按顺序介绍自己工作；  

  * 项目报告要点  
    
    * 项目任务及研发过程  
    
    * 项目组及成员分工安排  
    
    * 项目组进度和里程碑（从项目启动算起）  
    
    * 项目开发过程中不同阶段采用的关键技术（老师推荐的8次课中讲到的内容或项目组自行采纳的其他技术）  
    
    * 项目开发过程中使用的辅助工具  
    
    * 项目相关工作量统计数据（需求功能点、各类文档规模／页数、代码行、发现和修复的缺陷数）  
    
    * 项目研发过程中的变更及应对情况（变更的来源包括老师提出的变更要求、项目组自行提出的变更；变更的类型包括软件生存期各阶段针对任务、技术、人员等相关的变更）  
    
    * 项目组能够体现项目管理、过程管理、配置管理、质量管理的相关活动和结果（如开会、指定代码规范、文档规范、使用相关协同工具等等）  
    
  * 个人报告要点  
  
    * 个人任务  
    
    * 本课程学习的软件工程理论、方法和技术  
    
    * 项目开发过程过程中学习的技术和工具（老师推荐的8次课中讲到的内容或自行采纳的其他技术）  
    
    * 项目开发过程中使用的辅助工具（选择项目开发场景展示任意2种工具使用的视频，不超过5分钟）  
    
    * 个人相关工作量统计数据（自己完成的各类文档规模／页数、代码行、发现和修复的缺陷数）  
    
    * 能够体现自己参与项目管理、过程管理、配置管理、质量管理的相关活动和结果  
    
    
三、系统和能力演示：  

  * 演示部分分项目演示和个人能力展示两个部分，请在准备验收的机器上准备好所有系统和能力展示所需资源;  
  
  * 项目演示：系统demo，可以播放录播视频或现场演示，后者加分，不超过15分钟；  
  
  * 个人工具使用能力展示： 列出在项目开发过程中使用的辅助工具，老师指定任意工具，选择项目开发任意场景展示所选工具使用，不超过5分钟；  
  
  * 个人项目成果展示：打开自己完成的代码或文档，解释考核老师指定代码或文档的相关片段；  
  
  
