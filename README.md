
目标：为中文自然语言处理领域发展贡献语料
-------------------------------------------------------------------------

#### 方式：贡献中文语料，请联系:nlp_chinese_corpus@163.com


#### 维基百科(wiki2019zh) ---- 百科类问答(baike2018qa) ---- 新闻语料(news2016zh)

1.维基百科json版(wiki2019zh)
-------------------------------------------------------------------------

#### 104万个词条(1,043,224条; 原始文件大小1.7G，压缩文件519M；数据更新时间：2019.2.7)

<a href="https://pan.baidu.com/s/1uPMlIY3vhusdnhAge318TA">维基百科-中文简体-json版【下载】</a>

可能的用途：可以做为通用中文语料，做预训练的语料或构建词向量，也可以用于构建知识问答。

结构：

{"id":<id>,"url":<url>,"title":<title>,"text":<text>} 其中，title是词条的标题，text是正文；通过"\n\n"换行。

例子：

    {"id": "53", "url": "https://zh.wikipedia.org/wiki?curid=53", "title": "经济学", "text": "经济学\n\n经济学是一门对产品和服务的生产、分配以及消费进行研究的社会科学。西方语言中的“经济学”一词源于古希腊的。\n\n经济学注重的是研究经济行为者在一个经济体系下的行为，以及他们彼此之间的互动。在现代，经济学的教材通常将这门领域的研究分为总体经济学和个体经济学。微观经济学检视一个社会里基本层次的行为，包括个体的行为者（例如个人、公司、买家或卖家）以及与市场的互动。而宏观经济学则分析整个经济体和其议题，包括失业、通货膨胀、经济成长、财政和货币政策等。..."}

效果：

    经济学
    经济学是一门对产品和服务的生产、分配以及消费进行研究的社会科学。西方语言中的“经济学”一词源于古希腊的。
    经济学注重的是研究经济行为者在一个经济体系下的行为，以及他们彼此之间的互动。在现代，经济学的教材通常将这门领域的研究分为总体经济学和个体经济学。微观经济学检视一个社会里基本层次的行为，包括个体的行为者（例如个人、公司、买家或卖家）以及与市场的互动。而宏观经济学则分析整个经济体和其议题，包括失业、通货膨胀、经济成长、财政和货币政策等。
    其他的对照还包括了实证经济学（研究「是什么」）以及规范经济学（研究「应该是什么」）、经济理论与实用经济学、行为经济学与理性选择经济学、主流经济学（研究理性-个体-均衡等）与非主流经济学（研究体制-历史-社会结构等）。
    经济学的分析也被用在其他各种领域上，主要领域包括了商业、金融、和政府等，但同时也包括了如健康、犯罪、教育、法律、政治、社会架构、宗教、战争、和科学等等。到了21世纪初，经济学在社会科学领域各方面不断扩张影响力，使得有些学者讽刺地称其为「经济学帝国主义」。
    在现代对于经济学的定义有数种说法，其中有许多说法因为发展自不同的领域或理论而有截然不同的定义，苏格兰哲学家和经济学家亚当·斯密在1776年将政治经济学定义为「国民财富的性质和原因的研究」，他说：
    让-巴蒂斯特·赛伊在1803年将经济学从公共政策里独立出来，并定义其为对于财富之生产、分配、和消费的学问。另一方面，托马斯·卡莱尔则讽刺的称经济学为「忧郁的科学」（Dismal science），不过这一词最早是由马尔萨斯在1798年提出。约翰·斯图尔特·密尔在1844年提出了一个以社会科学定义经济学的角度：
    .....

<img src="https://github.com/brightmart/nlp_chinese_corpus/blob/master/resources/wiki_zh.jpg"  width="90%" height="90%" />



2.百科类问答json版(baike2018qa)
-------------------------------------------------------------------------

#### 150万个问答( 原始数据1G多，压缩文件663M；数据更新时间：2018年)

<a href='https://pan.baidu.com/s/12TCEwC_Q3He65HtPKN17cA'>点此下载</a>，密码:fu45


#### 数据描述

含有150万个问题和答案，每个问题属于一个类别。总共有492个类别，其中频率达到或超过10次的类别有434个。

数据集划分：数据去重并分成三个部分。训练集：142.5万；验证集：4.5万；测试集，数万，不提供下载。

可能的用途：可以做为通用中文语料，训练词向量或做为预训练的语料；也可以用于构建百科类问答；其中类别信息比较有用，可以用于做监督训练，从而构建

更好句子表示的模型、句子相似性任务等。

结构：

    {"qid":<qid>,"category":<category>,"title":<title>,"desc":<desc>,"answer":<answer>}
    
    其中，category是问题的类型，title是问题的标题，desc是问题的描述，可以为空或与标题内容一致。

例子：
    
    {"qid": "qid_2540946131115409959", "category": "生活知识", "title": "冬天进补好一些呢，还是夏天进步好啊？ ", "desc": "", "answer": "你好！\r\r当然是冬天进补好的了，夏天人体的胃处于收缩状态，不适宜大量的进补，所以我们有时候说：“夏天就要吃些清淡的，就是这个道理的。”\r\r不过，秋季进补要注意“四忌” 一忌多多益善。任何补药服用过量都有害。认为“多吃补药，有病治病，无病强身”是不的。过量进补会加重脾胃、肝脏负担。在夏季里，人们由于喝冷饮，常食冻品，多有脾胃功能减弱的现象，这时候如果突然大量进补，会骤然加重脾胃及肝脏的负担，使长期处于疲弱的消化器官难于承受，导致消化器官功能紊乱。 \r\r二忌以药代食。重药物轻食物的做法是不科学的，许多食物也是好的滋补品。如多吃荠菜可治疗高血压；多吃萝卜可健胃消食，顺气宽胸；多吃山药能补脾胃。日常食用的胡桃、芝麻、花生、红枣、扁豆等也是进补的佳品。\r\r三忌越贵越好。每个人的身体状况不同，因此与之相适应的补品也是不同的。价格昂贵的补品如燕窝、人参之类并非对每个人都适合。每种进补品都有一定的对象和适应症，应以实用有效为滋补原则，缺啥补啥。 \r\r四忌只补肉类。秋季适当食用牛羊肉进补效果好。但经过夏季后，由于脾胃尚未完全恢复到正常功能，因此过于油腻的食品不易消化吸收。另外，体内过多的脂类、糖类等物质堆积可能诱发心脑血管病。"}
  

<img src="https://github.com/brightmart/nlp_chinese_corpus/blob/master/resources/baike_qa.png"  width="100%" height="100%" />


#### 公开评测：

欢迎报告模型在验证集上的准确率。任务1： 类别预测。

报告包括：#1）验证集上准确率；#2）采用的模型、方法描述、运行方式，1页PDF；#3）可运行的源代码(可选)

基于#2和#3，我们会在测试集上做测试，并报告测试集上的准确率；只提供了#1和#2的队伍，验证集上的成绩依然可以被显示出来，但会被标记为未验证。


3.新闻语料json版(news2016zh)
-------------------------------------------------------------------------

#### 250万篇新闻( 原始数据9G，压缩文件3.6G；新闻内容跨度：2014-2016年)

<a href=''>点此下载</a>，密码: 

#### 数据描述

包含了250万篇新闻。新闻来源涵盖了6.3万个媒体，含标题、关键词、描述、正文。

数据集划分：数据去重并分成三个部分。训练集：243万；验证集：7.7万；测试集，数万，不提供下载。

可能的用途：

    可以做为【通用中文语料】，训练【词向量】或做为【预训练】的语料；
   
    也可以用于训练【标题生成】模型，或训练【关键词生成】模型（选关键词内容不同于标题的数据）；

    亦可以通过新闻渠道区分出新闻的类型。

结构：

    {'news_id': <news_id>,'title':<title>,'content':<content>,'source': <source>,'time':<time>,'keywords': <keywords>,'desc': <desc>, 'desc': <desc>}

    其中，title是新闻标题，content是正文，keywords是关键词，desc是描述，source是新闻的来源，time是发布时间

例子：
    
    {"news_id": "610130831", "keywords": "导游，门票","title": "故宫淡季门票40元 “黑导游”卖外地客140元", "desc": "近日有网友微博爆料称，故宫午门广场售票处出现“黑导游”，专门向外地游客出售高价门票。昨日，记者实地探访故宫，发现“黑导游”确实存在。窗口出售", "source": "新华网", "time": "03-22 12:00", "content": "近日有网友微博爆料称，故宫午门广场售票处出现“黑导游”，专门向外地游客出售高价门票。昨日，记者实地探访故宫，发现“黑导游”确实存在。窗口出售40元的门票，被“黑导游”加价出售，最高加到140元。故宫方面表示，请游客务必通过正规渠道购买门票，避免上当受骗遭受损失。目前单笔门票购买流程不过几秒钟，耐心排队购票也不会等待太长时间。....再反弹”的态势，打击黑导游需要游客配合，通过正规渠道购买门票。"}
  

<img src="https://github.com/brightmart/nlp_chinese_corpus/blob/master/resources/news2016zh.png"  width="100%" height="100%" />


Contribution/贡献语料
-------------------------------------------------------------------------

贡献中文语料，请发送邮件至nlp_chinese_corpus@163.com

add your chinese corpus here by sending us an email



Reference
-------------------------------------------------------------------------

1. <a href='https://github.com/AimeeLee77/wiki_zh_word2vec'>利用Python构建Wiki中文语料词向量模型试验</a>

2. <a href='https://github.com/attardi/wikiextractor'>A tool for extracting plain text from Wikipedia dumps</a>

3. <a href='https://github.com/yichen0831/opencc-python'>Open Chinese convert (OpenCC) in pure Python:開放中文轉換</a>

4. <a href='https://dumps.wikimedia.org/zhwiki/latest/'>dumps of wiki, latest in chinese</a>


