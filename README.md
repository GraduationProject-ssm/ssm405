# [首页查询更多项目](https://github.com/GraduationProject-ssm) 包安装运行


# ssm405基于java web的商铺租赁管理系统的设计与实现+jsp

![picture](https://raw.githubusercontent.com/GraduationProject-springboot/.github/main/img/wx.png)

### 点击播放视频 ▼
[![Watch the video](https://i.sstatic.net/Vp2cE.png)](https://www.bilibili.com/video/BV1t58veLEnL?p=5)


# 第1章 绪论
## 1.1选题动因
当前的网络技术，软件技术等都具备成熟的理论基础，市场上也出现各种技术开发的软件，这些软件都被用于各个领域，包括生活和工作的领域。随着电脑和笔记本的广泛运用，以及各种计算机硬件的完善和升级，市面上的电脑和笔记本的性能都得到提升，可以支持的软件也逐渐增多，因此，在计算机上安装软件来发挥其高效地信息处理的作用，则很受人们的青睐。对于商铺租赁信息来讲，通过手工形式处理，在面对庞大的信息数量时，就显得不适宜了，首先需要花费的时间比较多，其次数据出错率比较高，而且对错误的数据进行更改也比较困难，最后，检索数据费事费力。因此，为了解决上述问题，有必要建立商铺租赁管理系统，来规范商铺租赁信息管理流程，让管理工作可以系统化和程序化，同时，商铺租赁管理系统的有效运用可以帮助管理人员准确快速地处理信息。
## 1.2目的和意义
商铺租赁管理系统可以对商铺租赁信息进行集中管理，可以真正避免传统管理的缺陷。商铺租赁管理系统是一款运用软件开发技术设计实现的应用系统，在信息处理上可以达到快速的目的，不管是针对数据添加，数据维护和统计，以及数据查询等处理要求，商铺租赁管理系统都可以轻松应对。所以，商铺租赁管理系统的运用是让商铺租赁信息管理升级的最好方式。它可以实现信息处理的便利化要求，还可以规范信息处理的流程，让事务处理成为管理人员手中的一件简单事，而不是之前手工处理时的困难事。尽管商铺租赁管理系统具备较完善的功能，但是也需要管理人员利用闲暇时间提升自身素质以及个人能力，在操作商铺租赁管理系统时可以最大化运用商铺租赁管理系统提供的功能，让系统在满足高效率处理数据的同时，也能始终稳定运行，还可以确保数据的可靠性与数据处理的质量。
## 1.3论文结构安排
本文总共分为6个章节，每个章节都对本系统描述了不同的内容。接下来就对本文的研究内容进行阐述。

第1章：这个章节是论文的绪论部分。从选题的背景和意义的角度阐述即将开发的系统。

第2章：这个章节是技术介绍部分。从本系统需要运用的技术知识的角度阐述系统。

第3章：这个章节是系统分析部分。从分析系统可行性，分析系统功能和性能等角度阐述系统。

第4章：这个章节是系统设计部分。从系统功能结构的角度和数据库设计的角度阐述系统。

第5章：这个章节是系统实现部分。从系统功能模块运行效果的角度阐述系统。

第6章：这个章节是系统测试部分。从测试系统功能，系统测试方法的角度阐述系统。


# 第2章 开发环境与技术
开发商铺租赁管理系统需要搭建编程的环境，也需要通过调查，对各个相关技术进行分析，选取适合本系统开发的技术与工具。
## 2.1 MYSQL数据库
题目确定了是一个应用程序之后，就开始按部就班的进行设计与分析。本课题是需要数据库作为数据管理工具以及数据载体，从程序功能分析到数据分析，选择合适的关系型数据库是当下所选择的重要环节。关系型数据库可选择余地不多，本身甲骨文公司的两个，微软的两个，IBM的一个，也就是这五个了，功能和差异都不影响数据库的选择，因为这些数据库都能实现应用程序功能所需的，那么只能从其他的方面来综合考虑哪种数据库更合适。作为开发使用的电脑硬件上来讲，还是大一的时候买的，当初并没有太多的钱买好一点的电脑，只是作为学习用的，所以经过这么几年的使用，电脑老化了，性能下降也比较厉害，还有好多需要用的学习资料，本身面临毕业，选择学校机房也不是一个长久的打算，选择一个数据库适合自己的老旧笔记本电脑作为学习开发当前的应用，是最重要的。综合考虑的结果就是选用MySQL数据库作为应用数据库，因为MySQL数据库体积小，占用内存小，不影响电脑上其他用的软件运行，并且不需要因为安装维护MySQL数据库而重装系统，最终选择的数据库就是MySQL数据库。
## 2.2 Tomcat 介绍
刚开始学习Java语言的时候，是不知道还有Tomcat这些东西的，各种语法各种输出在控制台进行输出结果，当Java网站开发的时候就不可避免的学习到了Tomcat服务器。Tomcat准确的来讲不算是服务器，可以说是JSP引擎或者一个容器，这些都是学术上或者原理上都比较贴切的，但是实际工作中Tomcat就是作为一个web服务器来用的，因为可以实现网站的发布和运行。因为工作原理的原因，Tomcat一般作为中小型企业和并发量并不突出的一种轻量级的服务器存在的，比如某些行业的应用系统，本身客户端就不多，需要的连接也不多，一般都用Tomcat的。Tomcat里面可以配置多个网站，配置文件后缀是config的文档，类似于XML的结构，比较清晰明了。每当Java发布新的版本的时候，Tomcat也会为了匹配Java的版本进行升级，目前Tomcat版本已经到版本10了。Tomcat标识是一只有点发黄的小猫咪，当Tomcat配置成功一般测试的时候能看到这个小猫咪就算是成功的，才能进行下一步的配置。Tomcat服务器在Java网站开发中还是挺合适的。
## 2.3 JSP技术
JSP技术可以让初学者尽快上手进行编写动态网站，不需要变成高级的Java编程人员才可以书写代码，从学习的效率还有编写的效率上都有很大的提升。让着重于网页开发者与着重于后台逻辑开发进行分离合作开发变成了一种可能，降低了学习成本，不需要考虑程序运行解释编译阶段的话，JSP网页本身就可以理解成一个普通的Servlet。JSP结构上面，主要分为两个方面，一个是专属的JSP引擎，通俗的讲就是可以实现JSP编译后运行解释的一个东西，另一个就是web服务器。JSP运行编译需要JSP引擎和web服务器进行配合以及相互协作，当然他们的分工也是很明确的，这样才可以真正的运行起来。JSP容器和引擎有Tomcat，这个Tomcat其实也还有Apache静态解释代码的部分，虽然看起来运行效果差不多，但是其实是两个截然不同的工具，在文件系统里目录也是不一样的，当然如果有特殊需求也是可以进行特殊的配置的，配置上面还是比较灵活的。虽然Tomcat部署了网站之后就可以运行网页让客户访问，但是Tomcat也只是JSP引擎而非web服务器。比如JRUN和Resin都算是JSP引擎，而web服务器的职责比较单一，就是处理客户端请求还有返回给客户显示请求处理后的数据而已。JSP引擎则可以运行纯HTML编写的网站，也可以运行JSP编写的动态网站，在效率上也只是比单纯的web服务器而已，但是从纯web服务器无法运行动态网站上来讲，JSP引擎在功能上还是强大了很多，提升一点点效率反而算不了什么，对于必须实现的功能这些要素上，选择了JSP技术。


# 第3章 系统分析
用户的需求以及与本系统相似的在市场上存在的其它系统可以作为系统分析中参考的资料，分析人员可以根据这些信息确定出本系统具备的功能，分析出本系统具备的性能等内容。
## 3.1可行性分析
尽管系统是根据用户的要求进行制作，但是在确定制作前，有必要分析其可行性。
### 3.1.1操作可行性分析
开发本系统需要用到的工具，本人都比较熟悉，因此可以使用这些工具，完整开发商铺租赁管理系统。此外，商铺租赁管理系统在功能上，基本都是完成信息的处理，涵盖了添加，修改，删除等，而且操作者面对的都是各个功能操作界面，并不是编码后台，所以一般的使用者都可以通过操作界面轻松完成信息的加工处理。因此，本系统操作可行。
### 3.1.2经济可行性分析
开发本系统，并没有投入资金购买开发工具。因为使用的开发工具都是事先在百度上下载安装在本人电脑上的，随着软件开发技术的成熟，系统功能实现的编码也都模块化，很容易通过各大软件开发类网站获取，并通过小部分代码改动，运用到本系统中，这些都不需要资金投入，同时，本系统开发的结构选用B/S，成本可以忽略不计。
### 3.1.3技术可行性分析
本系统需要的软件包括Eclipse，Tomcat，Mysql等，这些工具都接触并使用过，至于JAVA，B/S，Jsp，Html等技术，图书馆都有对应的书籍可以参考学习，加上平时课堂上学习的编程小项目对这些技术都有讲解，另外，本人也从课程设计作业中锻炼了编程能力。所以在技术上，可以完成商铺租赁管理系统的编程开发。

通过上面的分析，已经确定了本系统在经济上的可行，本系统在技术上的可行，本系统在操作上的可行。由此，可以得出在目前的条件下，对于商铺租赁管理系统的设计与实现是可以进行下去的。
## 3.2系统流程分析
本系统在处理数据时，其内部的操作逻辑也需要使用相应的工具进行展示。

在本系统的数据录入页面，对于操作者提供的每条数据都有相应的检验规则，比如数据信息不能有非法字符，或者本来应该是汉字的数据，不能用字母代替，还有对数据内容的长度等进行规范，这样的可以确保数据准确性的检验规则，在编码时，就提前编写好了。数据添加的流程见下图。如果数据已经保存进入数据库，则说明操作者提供的数据内容和格式都是符合要求的。

![](/md/blog.001.png)

图3.1 添加信息流程图

很多时候，面对系统中的大量数据，难免会发现一些错误，因此需要及时纠正错误，本系统也提供数据后期的修改功能，其流程见下图。但是更新的数据也需要通过数据有效性检验。能够最终写入数据库则说明修改的数据是符合要求的。

![](/md/blog.002.png)

图3.2 修改信息流程图

面对数据库里面大量数据，在系统的前台，要想快速获取需要的信息，就需要使用查询功能。其流程见下图。该功能需要操作者提前输入关键词，当系统的后台数据库保存了与关键词匹配的数据时，就会及时显示出来，整个过程耗时很短。

![](/md/blog.003.png)

图3.3 查询信息流程图
## 3.3系统性能分析
分析商铺租赁管理系统对于性能的需求主要还是从下面的5个角度来分析，它们分别是系统的实用性，系统的适应性，系统的易操作性，系统的安全性和系统的易维护性。

性能需求一：系统的实用性，本系统主要是让管理人员集中处理相关信息，可以提供方便快捷的信息添加，信息编辑等操作。在提高信息管理人员的工作效率的同时，也可以降低管理成本，并大大减少管理人员日常繁琐的工作量。

性能需求二：系统的适应性，本系统对于运行环境的要求并不高，可以被广泛运用在生活中。因为使用者只要在日常使用的计算机，或者是随身携带的笔记本上搭建运行环境都能运行本系统，另外系统提供的基础功能包括添加，修改等都能随时操作。

性能需求三：系统的易操作性，本系统提供的功能跟同类型系统一样，也具备简单的增删改操作，操作流程的逻辑也符合广大使用者的使用需求，使用者使用本系统管理数据会非常顺手。

性能需求四：系统的安全性，本系统在数据保存与管理上安全系数要达标，在设计与编码阶段，通过对用户进行权限分配，把系统的功能依照不同用户的角色进行分配，在首次进入系统时，通过编写安全验证的代码模块，引导不同用户进入不同的操作界面。还可以对用户基础信息包括登录的账号密码等进行加密保存，可以利用当下常用的技术成熟的MD5加密技术实现。

性能需求五：系统的易维护性，本系统在后期运行中，会根据使用者的操作，产生许多数据信息，为了便于维护，就要求这些数据可以通过工具从数据库中导出来，对于一些阶段性数据，可以进行批量删除，以此达到轻负荷处理数据的目标，让本系统可以变得更加轻盈。
## 3.4系统功能分析
完成这部分内容，需要设计人员提前做好准备工作，包括对系统的实际使用人员进行调研，获取他们对本系统的功能需求，也需要通过参考和分析大量文献，获取同类系统的功能，由此分析得出本系统的功能。

管理员是本系统的一个角色，其用例见下图。管理员管理房东，管理公告，管理商铺出租，租赁合同等信息。

![](/md/blog.004.png)

图3.4 管理员用例图

房东是本系统的一个角色，其用例见下图。房东审核商铺出租订单，添加租赁合同，管理商铺出租信息。

![](/md/blog.005.png)

图3.5 房东用例图

用户是本系统的一个角色，其用例见下图。用户租赁商铺，查看公告，查看商铺租赁订单，查看租赁合同信息。

![](/md/blog.006.png)

图3.6 用户用例图


# 第4章 系统设计
市面上设计比较好的系统都有一个共同特征，就是主题鲜明突出。通过对页面简洁清晰的布局，让页面的内容，包括文字语言，或者视频图片等元素可以清晰表达出系统的主题。让来访用户无需花费过多精力和时间找寻需要的内容。
## 4.1界面设计原则
一般来说，大部分用户使用系统，有些是想从系统中获取需要的信息，有些则是使用系统提供的服务。所以，为了改善用户体验，提高系统的使用率，在对系统界面设计时，需要按照下面的原则进行。

第一点，对用户进行分析，了解用户使用系统的目的，以及使用系统的方式，考虑大部分用户的阅读习惯，设计Z字形或F型结构可以方便用户获取信息。

第二点：设计有效的导航，这个包括每个页面上都有导航条的显示，有时也可以在页面的底部设计导航条，当用户进入具体页面时，要设计相应的位置提示，在页面中比较特殊的位置，需要设计返回链接，可以返回上个页面，也可以返回首页等。

第三点：对整个系统要运用统一的设计方案，包括色彩方案的一致性，页面模板的相似性等，对相同操作和专业术语的描述在整个系统中也应该保持一致。

第四点：设计的界面要保证传达的内容清晰准确。要避免在同一个页面设计非常多的内容，另外可以准确对系统内容进行分类，把页面中用户视觉集中的位置，用来显示重要信息。

作为初学者，并没有那么多的设计经验，但是可以运用上面提到的界面设计原则设计出比较好的系统，可以让用户产生良好的使用体验。
## 4.2功能结构设计
为了让系统的编码可以顺利进行，特意对本系统功能进行细分设计，管理员的功能在经过细分后，设计的功能结构见下图。管理员管理房东，管理公告，管理商铺出租，租赁合同等信息。 

![](/md/blog.007.png)

图4.1 管理员功能结构图

房东的功能在经过细分后，设计的功能结构见下图。房东审核商铺出租订单，添加租赁合同，管理商铺出租信息。

![](/md/blog.008.png)

图4.2 房东功能结构图

用户的功能在经过细分后，设计的功能结构见下图。用户租赁商铺，查看公告，查看商铺租赁订单，查看租赁合同信息。

![](/md/blog.009.png)

图4.3 用户功能结构图
## 4.3数据库设计
一般来说，对用户进行调查，了解其需求，主要还是完成功能上的分析设计，殊不知，设计功能时，也要展示对数据库的设计。数据库服务于程序，它可以按照设定的规则对程序的数据进行保存，因此，也可以说数据库就是程序相关数据的集合。为了保证程序的高质量，数据库提供的数据存储服务也需要快速响应，同时数据信息也要安全合法可靠，所以设计一个数据库这样的任务也需要高度重视，并花时间和精力去努力完成。毕竟这影响到后期程序的开发和使用。试想而知，假设设计一个不好的数据库，遇到的问题将会有：第一，面对信息处理，会有着繁琐的业务逻辑，延长事务处理时间。第二：程序编码期间，将会产生更多的代码去完成数据处理的功能，产生大量的数据冗余，而且也不方便注释代码，还会占用更多的存储空间。综上所述，设计出合理的数据库是多么的重要。
### 4.3.1数据库概念设计
完成此部分内容，需要通过设计展示最终的数据库概念模型，因为这是数据库设计中的关键。而这个概念模型也是在数据库设计中必不可少的E-R模型。之所以要运用E-R模型展示概念设计的内容，主要还是因为E-R模型可以更加方便的展示实体，还有实体间的关系，而且E-R模型可以更方便表达数据的意义。这将有助于数据库的设计工作。

E-R模型的建立也需要使用对应的软件，目前市场上使用频率高的是微软旗下的成员之一Visio,当然，国产的亿图软件也可以绘制E-R模型。无论是采用哪个绘制软件，要绘制好E-R图，还是要掌握E-R图的各个符号代表的意义。比如矩形常用来表示实体，对于实体的特征就使用椭圆形符号表示，像菱形这样的符号就是处于两个矩形之间，代表着实体间的联系，而直线符号就是把矩形，椭圆，菱形这些符号进行连接。接下来就对本系统的E-R图进行展示。

（1）设计的商铺出租实体，其具备的属性见下图。

![](/md/blog.010.png)

图4.4 商铺出租实体属性图

（2）设计的用户实体，其具备的属性见下图。

![](/md/blog.011.png)

图4.5 用户实体属性图

（3）设计的房东实体，其具备的属性见下图。

![](/md/blog.012.png)

图4.6 房东实体属性图

4. 设计的合同实体，其具备的属性见下图。

![](/md/blog.013.png)

图4.7 合同实体属性图

4. 设计的上述实体间关系见下图。

![](/md/blog.014.png)

图4.8 实体间关系E-R图
### 4.3.2 数据库物理设计
作为程序后台的支持，本数据库也需要设计数据存储的结构。而数据存储结构的设计就包括了数据表结构的设计和创建。这里也会运用到前面设计的E-R模型来构建数据表结构。

数据表结构包括了字段，数据类型，还有字段的取值范围等信息。而E-R模型中的实体就是一张表，实体的特征就可以作为该表中的字段，根据本程序信息存储要求，设计每个字段需要的类型，还有该字段的取值范围等。每当设计完成一张数据表，就需要及时保存在数据库里面，并对该设计的数据表准确命名，要求设置的数据表的名称尽量不要是中文，而且要方便记忆。因为在程序编码阶段，通过SQL语句可以把程序里面的数据写入在各个数据表里面，而这个环节需要使用到数据表的名称。如果数据表名称是中文的话，可能会乱码并影响程序运行。下面就以表格形式展示设计的结果。

` `表4.1商铺出租信息表

|字段|类型|空|默认|注释|
| :-: | :-: | :-: | :-: | :-: |
|id (主键)|int(11)|否||主键|
|chuzu\_name|varchar(200)|是|NULL|商铺名称 |
|huixing\_types|int(255)|是|NULL|户型 |
|chuzu\_mianji|decimal(10,4)|是|NULL|面积|
|chuzu\_money|decimal(10,4)|是|NULL|价格/月|
|chuzu\_photo|varchar(200)|是|NULL|图片|
|chuzu\_weizhi|varchar(200)|是|NULL|位置|
|fangdong\_id|int(200)|是|NULL|发布房东|
|chuzu\_types|int(200)|是|NULL|商铺状态 |
|chuzu\_content|text|是|NULL|详细信息|
|insert\_time|timestamp|是|NULL|录入时间|
|create\_time|timestamp|是|NULL|创建时间 |
` `表4.2商铺出租留言信息表 

|字段|类型|空|默认|注释|
| :-: | :-: | :-: | :-: | :-: |
|id (主键)|int(11)|否||主键|
|chuzu\_id|int(11)|是|NULL|商铺出租id|
|yonghu\_id|int(11)|是|NULL|用户id|
|chuzu\_liuyan\_content|text|是|NULL|留言内容|
|reply\_content|text|是|NULL|回复内容|
|insert\_time|timestamp|是|NULL|讨论时间|
|create\_time|timestamp|是|NULL|创建时间|


表4.3商铺出租订单信息表 

|字段|类型|空|默认|注释|
| :-: | :-: | :-: | :-: | :-: |
|id (主键)|int(11)|否||主键|
|chuzu\_id|int(11)|是|NULL|商铺出租id|
|yonghu\_id|int(11)|是|NULL|用户id|
|chuzu\_order\_day|int(255)|是|NULL|租赁时间/年 |
|shenhe\_types|int(255)|是|NULL|审核|
|chuzu\_order\_money|decimal(10,4)|是|NULL|总价|
|insert\_time|timestamp|是|NULL|订单创建时间|
|create\_time|timestamp|是|NULL|创建时间|
` `表4.4房东信息表 

|字段|类型|空|默认|注释|
| :-: | :-: | :-: | :-: | :-: |
|id (主键)|int(11)|否||主键|
|username|varchar(200)|是|NULL|账户|
|password|varchar(200)|是|NULL|密码|
|fangdong\_name|varchar(200)|是|NULL|房东姓名 |
|sex\_types|int(11)|是|NULL|性别|
|fangdong\_id\_number|varchar(200)|是|NULL|身份证号|
|fangdong\_phone|varchar(200)|是|NULL|手机号|
|fangdong\_photo|varchar(200)|是|NULL|照片|
|create\_time|timestamp|是|NULL|创建时间|
` `表4.5 合同信息表

|字段|类型|空|默认|注释|
| :-: | :-: | :-: | :-: | :-: |
|id (主键)|int(11)|否||主键|
|hetong\_name|varchar(255)|是|NULL|合同名称 |
|yonghu\_id|int(11)|是|NULL|签订用户|
|fangdong\_id|int(11)|是|NULL|发布房东|
|hetong\_file|varchar(255)|是|NULL|合同|
|hetong\_content|text|是|NULL|合同简介|
|insert\_time|timestamp|是|NULL|签订时间|
|create\_time|timestamp|是|NULL|创建时间|




表4.6公告信息表 

|字段|类型|空|默认|注释|
| :-: | :-: | :-: | :-: | :-: |
|id (主键)|int(11)|否||主键|
|news\_name|varchar(200)|是|NULL|公告名称 |
|news\_types|int(11)|是|NULL|公告类型 |
|news\_photo|varchar(200)|是|NULL|公告图片|
|insert\_time|timestamp|是|NULL|公告时间|
|news\_content|text|是|NULL|公告详情|
|create\_time|timestamp|是|NULL|创建时间|
` `表4.7管理员信息表

|字段|类型|空|默认|注释|
| :-: | :-: | :-: | :-: | :-: |
|id (主键)|bigint(20)|否||主键|
|username|varchar(100)|否||用户名|
|password|varchar(100)|否||密码|
|role|varchar(100)|是|管理员|角色|
|addtime|timestamp|否|CURRENT\_TIMESTAMP|新增时间|
` `表4.8 用户信息表 

|字段|类型|空|默认|注释|
| :-: | :-: | :-: | :-: | :-: |
|id (主键)|int(11)|否||主键|
|username|varchar(200)|是|NULL|账户|
|password|varchar(200)|是|NULL|密码|
|yonghu\_name|varchar(200)|是|NULL|用户姓名 |
|sex\_types|int(11)|是|NULL|性别|
|yonghu\_id\_number|varchar(200)|是|NULL|身份证号|
|yonghu\_phone|varchar(200)|是|NULL|手机号|
|yonghu\_photo|varchar(200)|是|NULL|照片|
|create\_time|timestamp|是|NULL|创建时间|


# 第5章 系统实现
这个环节需要使用前面的设计方案，包括对系统模块的设计，还有对程序后台的数据支持的数据库的设计等。不过这部分内容还是强调系统编码人员的开发能力，要把前面设计的内容通过编码的形式以一个完整的，可以运行的系统呈现出来。
## 5.1管理员功能实现
### 5.1.1房东管理
管理员管理房东，其运行效果见下图。在本页面，管理员可以为房东重置密码，可以修改房东的手机号，照片，姓名等信息，也可以删除房东信息。

![](/md/blog.015.png)

图5.1房东管理页面
### 5.1.2公告管理
管理员管理公告。其运行效果见下图。公告信息的管理是管理员负责的内容，管理员需要发布公告，查询公告，修改公告信息。

![](/md/blog.016.png)

图5.2 公告管理页面
### 5.1.3用户管理
管理员可以管理用户，其运行效果见下图。管理员能够对用户的登录密码进行重置，可以修改用户的注册信息。

![](/md/blog.017.png)

图5.3 用户管理页面
## 5.2 房东功能实现
### 5.2.1商铺出租管理
房东管理商铺出租信息。其运行效果见下图。房东对需要出租的商铺信息进行登记，可以通过商铺名称查询商铺信息，可以修改商铺的状态，位置，面积，户型等信息。

![](/md/blog.018.png)

图5.4 商铺出租管理页面
### 5.2.2商铺出租订单管理
房东管理商铺出租订单，其运行效果见下图。用户租赁商铺，该商铺的房东需要在当前模块进行出租订单的审核。

![](/md/blog.019.png)

图5.5 商铺出租订单管理页面
### 5.2.3租赁合同管理
房东管理租赁合同，其运行效果见下图。房东在当前页面添加租赁合同信息，可以下载租赁合同文件，可以修改租赁合同的描述信息。

![](/md/blog.020.png)

图5.6 租赁合同管理页面
## 5.3 用户功能实现
### 5.3.1商铺出租
用户查看商铺出租。其运行效果见下图。用户查看出租的商铺介绍信息，可以在页面底部对出租的商铺进行留言，可以点击立即预订按钮对出租的商铺进行租赁。

![](/md/blog.021.png)

图5.7 商铺出租页面
### 5.3.2公告信息
用户查询公告信息，其运行效果见下图。用户通过公告名称，或者是通过公告类型可以查询公告。

![](/md/blog.022.png)

图5.8 公告信息页面
### 5.3.3商铺出租订单
用户查看商铺出租订单。其运行效果见下图。用户在本页面查看租赁的商铺的审核情况，查看房东是否同意把商铺出租给该用户。

![](/md/blog.023.png)

图5.9 商铺出租订单页面
### 5.3.4租赁合同管理
用户查看租赁合同。其运行效果见下图。用户在本页面查看租赁合同信息，下载租赁合同文件。

![](/md/blog.024.png)

图5.10 租赁合同管理页面






# 










