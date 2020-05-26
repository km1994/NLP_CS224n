# NLP组队学习 任务大纲

## 项目由来

Datawhale_NLP_CS224n 是由 Datawhale 组织成员 参考 微信公众号 [夕小瑶的卖萌屋](https://mp.weixin.qq.com/s?__biz=MzIwNzc2NTk0NQ==&mid=2247485633&idx=1&sn=24f65254ae07f53ebb1d976b37d2573b&chksm=970c2017a07ba90182d85fc0a238d3234bd9fe3eb357371db756ba73e321f733d52658fe941b&token=1203749132&lang=zh_CN#rd) 开源课程学习项目 [CS224N-winter-together](https://github.com/xixiaoyao/CS224n-winter-together) 所发起的 NLP开源课程学习项目。

## 项目动机

该项目主要为了 给那些**想入门NLP却没找到比较好的入门教程的 New NLPer** 提供 一个 学习视频索引、课程笔记分享、课后问题解答 的平台 ，以帮助他们入门 NLP。每个人均可将自己的笔记、感悟、作业等提交到该repo下面对应课程的文件夹底下，来方便大家参考学习，具体细节见[提交流程](https://github.com/xixiaoyao/CS224n-winter-together/blob/master/README.md#个人笔记感悟和作业提交流程)。另外，鼓励大家以markdown格式进行提交以免repo大小增长过快。

## 项目介绍

自然语言处理( NLP )是信息时代最重要的技术之一，也是人工智能的重要组成部分。NLP的应用无处不在，因为人们几乎用语言交流一切：网络搜索、广告、电子邮件、客户服务、语言翻译、医疗报告等。近年来，深度学习方法在许多不同的NLP任务中获得了非常高的性能，使用了不需要传统的、任务特定的特征工程的单个端到端神经模型。在本课程中，学生将全面了解NLP深度学习的前沿研究。通过讲座、作业和最终项目，学生将学习设计、实现和理解他们自己的神经网络模型的必要技能。

## 基本信息

- 学习名称：NLP组队学习
- 学习周期：12天
- 学习形式：视频学习+实践
- 人群定位：具备一定编程基础，有学习和梳理自然语言处理算法的需求
- 难度等级：中
- 先修组队学习：无
- 后续推荐组队学习：比赛强化
- 编程语言：不限

## 课程介绍

- Task 1: Introduction and Word Vectors （3天）
  - [slides](Lecture/Lecture1/slides/) 
  - [official notes](Lecture/Lecture1/official_notes/)
  - [youtube video](https://www.youtube.com/watch?v=8rXD5-xhemo)
  - [bilibili video](https://www.bilibili.com/video/BV1s4411N7fC?p=1)
  - [问题解答区](https://github.com/km1994/Datawhale_NLP_CS224n/issues/1)
  - 简介
    - 这一讲主要讲了NLP研究的对象，我们如何表示单词的含义，以及Word2Vec方法的基本原理。
  - [参考](Lecture/Lecture1/reference/)

- Task 2: Word Vectors and Word Senses （3天）
  - [slides](Lecture/Lecture2/slides/) 
  - [official notes](Lecture/Lecture2/official_notes/)
  - [youtube video](https://www.youtube.com/watch?v=kEMJRjEdNzM&list=PLoROMvodv4rOhcuXMZkNm7j3fVwBBY42z&index=2)
  - [bilibili video](https://www.bilibili.com/video/BV1s4411N7fC?p=2)
  - [问题解答区](https://github.com/km1994/Datawhale_NLP_CS224n/issues/2)
  - 简介
    - Task 1：Word Vector 主要介绍了Word2Vec模型，它是一种基于local context window的direct prediction预测模型，对于学习word vector，还有另一类模型是count based global matrix factorization，这一讲主要介绍了后一类模型以及Manning教 授组结合两者优点提出的 GloVe 模型。
  - [参考](Lecture/Lecture2/reference/)

- Task 3: Subword Models （3天）
  - [slides](Lecture/Lecture12/slides/) 
  - [official notes](Lecture/Lecture12/official_notes/)
  - [youtube video](https://www.youtube.com/watch?v=9oTHFx0Gg3Q&list=PLoROMvodv4rOhcuXMZkNm7j3fVwBBY42z&index=12)
  - [bilibili video](https://www.bilibili.com/video/BV1s4411N7fC?p=12)
  - [问题解答区](https://github.com/km1994/Datawhale_NLP_CS224n/issues/12)
  - 简介
    - 之前的 word2vec 和 glove 基本上都是基于word单词作为基本单位的，但是其缺点是不能很好的解决out-of-vocabulary即单词不在词汇库里的情况，且对于单词的一些词法上的修饰(morphology)处理的也不是很好。一个自然的想法就是能够利用比word更基本的组成来建立模型，以更好的解决这些问题。本节思考采用 n-gram 思想训练 word vector 模型，也就是 FastText。
  - [参考](Lecture/Lecture12/reference/)

- Task 4: Contextual Word Embeddings  （3天）
  - [slides](Lecture/Lecture13/slides/) 
  - [official notes](Lecture/Lecture14/official_notes/)
  - [youtube video](https://www.youtube.com/watch?v=kEMJRjEdNzM&list=PLoROMvodv4rOhcuXMZkNm7j3fVwBBY42z&index=13)
  - [bilibili video](https://www.bilibili.com/video/BV1s4411N7fC?p=13)
  - [问题解答区](https://github.com/km1994/Datawhale_NLP_CS224n/issues/13)
  - 简介
    - 之前的 Word Vector 如 Word2Vec, GloVe, fastText 等对每个单词仅有一种表示，而通常单词的含义依赖于其上下文会有所不同，而且每个单词不仅有一方面特征，而应有各方面特征如语义特征，语法特征等，这一讲集中讨论contextual word representation，主要比较了ELMO，GPT与BERT模型。
  - [参考](Lecture/Lecture13/reference/)

## 课程作业介绍

1. 英文词向量的探索
   - [作业链接](Assignments/official/homework1/en/)
   - [讨论区](https://github.com/km1994/Datawhale_NLP_CS224n/issues/21)
   
2. 中文词向量的探索
   - [作业链接](Assignments/official/homework1/zh/)
   - [讨论区](https://github.com/km1994/Datawhale_NLP_CS224n/issues/21) 
  
3. FastText 探索
   - [作业链接](Assignments/official/homework1/FastText/)
   - [讨论区](https://github.com/km1994/Datawhale_NLP_CS224n/issues/21) 

4. Bert 探索
   - [作业链接](Assignments/official/homework1/Bert/)
   - [讨论区](https://github.com/km1994/Datawhale_NLP_CS224n/issues/21) 

## 个人笔记、感悟和作业提交流程

请务必保证原创！若发现其他同学的笔记、作业等提交中有错误，鼓励提PR修复。另外，鼓励大家在上传的原创资料中留下联系方式，以便学习讨论和错误纠正。

提交流程：

- step 1. fork项目并将个人仓库中的项目git clone到本地。

- step 2. 在本地项目仓库中添加提交笔记、作业和课程项目到对应文件夹中，然后完成git add（文件添加）和git commit（本地提交）。

> 注意：cs224n的作业位于Assignments目录下，个人笔记和感悟位于FeatureNotes目录下，课程项目位于Project目录下。这三个目录均为开放性目录，每个人均可通过pull request来完成提交。提交细节请参考对应目录下的README文件。

- step 3. 在本地完成的提交后，通过git push将本地提交推送至自己的github远程仓库后，发起pull request。


## 致谢

1. [CS224n 课程主页](http://web.stanford.edu/class/cs224n/index.html)
2. [CS224n-winter-together](https://github.com/xixiaoyao/CS224n-winter-together)
3. [CS224n_winter2019_notes_and_assignments](https://github.com/lrs1353281004/CS224n_winter2019_notes_and_assignments)
  

