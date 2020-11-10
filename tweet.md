---
layout: tweet
title: tweet
permalink: /tweet/
published: published
---

*<2020-10-22 四>*
[十年IT灾难全面回顾和总结](https://www.csdn.net/article/2015-12-28/2826562)


什么是好的代码实现？逻辑结构清晰，层次错落有序
逻辑结构：
业务逻辑
模型逻辑
业务-模型适配逻辑



*<2020-10-16 Fri>*
打的一拳开，免得百拳来


*2019.11.11*
ldap 验证用户密码是否正确，需要使用 upn  或者 dn 作为用户名 https://github.com/Adldap2/Adldap2-Laravel/issues/580

*Sun Sep 29 20:34:46 CST 2019*
引用透明性 & 可重入性

[引用透明，最初是个数学概念，表示在同一作用域内，相同表达式的值相同](https://www.zhihu.com/question/52147030/answer/274972772)

[引用透明是指，在作用域内，x是多少，就永远是多少，所有引用x的表达式]( https://www.zhihu.com/question/52147030/answer/129190223)

`如果一个函数的输入相同，对应的计算结果也相同，那么它就具备「引用透明性」`  貌似是可重入性

*2016.08.08*
如果看起来是只鸭子，那就当成一只鸭子对待。

*2016.07.15*
消息队列的本质就是对信息有一对接口可以进行存取beanstalk ,redis 可以做的，mysql当然也可以做，只是效率问题而已


*2016.07.14*
Yii2 `Model` 子类里面定义了和数据库字段同名的公有属性，数据库对应的属性会被覆盖，无法给其赋值，更新。
可以使用 `\Yii::error(VarDumper::dumpAsString($model));` 查看一下对象值，就一目了然也。。


简繁体汉子匹配的正则 `[一-龠]`


*2016.07.11* tweet 开张了。。。

设计是自己的短板，还是借用别人的使用一下吧，样式抄自于  [http://www.yinwang.org/tweet.html](http://www.yinwang.org/tweet.html) ,并做了一点修改。
