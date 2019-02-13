DQU 综述
===

Index
---
<!-- TOC -->

- [Introduction](#introduction)
- [引用文献](#引用文献)

<!-- /TOC -->

<h3> 参考文献 </h3>
- (Prakash and Patel, 2015) Techniques for Deep Query Understanding


## Introduction

- 在过去的 20 年中，搜索查询的解释、处理以及向用户展示结果的方式一直在发生改变；
    - 从单纯基于文本匹配的检索到对查询的语义理解，包括上下文、位置、时间、用户之前的查询；

- 查询方式的改变：关键词查询（电脑，键盘输入） -> 自然语言查询（手持设备，语音输入）

**查询理解的应用**

- 上下文查询
    - 比如“Where can I eat cheese cake right now”，此时搜索引擎需要理解用户的意图、了解用户的位置以及当前的时间才能返回正确的结果

- 交互式问答查询
    - 返回准确的答案，比如“who is the president of USA now”
    - 当前查询可能与会话中的前一个问题有关

        <div align="center"><img src="./_assets/TIM截图20190212181144.png" height="" /></div>

        > 要实现上述示例，需要将第一个问题改为“who is the president of USA 2010”；因为目前（2019年）美国总统 Trump 有过三位妻子，所以第四个问题将无法返回正确结果；同理，如果搜索“who is the president of USA 2009”，那么到第二个问题就会出错，因为 2009 年美国总统换届，那年有两位总统。

    - 此时，查询理解模块必须考虑上下文，并从答案生成模块中获取上一个问题的目标实体，以理解查询。

- AI 个人助理
    - 微软 Cortana、苹果 Siri、Google Now
    - 他们必须了解哪些查询需要重定向到 Web 搜索引擎，哪些查询用于本地设备操作。


## 引用文献
- [2] Learning to Personalize Query Auto-Completion
    - 本文讨论了使用位置特征、年龄和性别等用户特征、区域特征、用户短历史特征和长历史特征进行查询自动完成的问题，并给出了使用该方法进行意图预测的思路。