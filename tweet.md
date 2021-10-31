---
layout: tweet
title: 只言片语
permalink: /tweet/
#published: published
published: true
---

## *<2021-10-31 日>* ##

`C-u C-c ! 使用当前时间插入非活动时间戳 org-time-stamp-inactive`


阅读的最重要重要的功用就是学习新词，如果感觉没有任何收获但至少也可以收获一些文字词语。


youtube-dl - 为什么在bilibili上用youtube-dl只能下载第一集视频？ 
https://www.coder.work/article/7568349
https://github.com/iawia002/annie


## *<2020-11-24 二>* ##

解决: LDAP-Unable to bind to server: Can't contact LDAP server 

https://zhuanlan.zhihu.com/p/32399005

## *<2020-11-22 日>* ##


今天备份照片，在想云盘给我备份的视频有原图和压缩两种，我在想一个什么样的结果，心里才会是你个让我比较满意的结果？

前些年用备份照片的时候，晕头转向的备份了一些照片，但是压缩的特别厉害，后来再看的时候，简直无法忍受，所以我就一直想着最好能原图给我备份，这是最好的，就是不失真，所谓的不失真，就是我的原始图片是什么就是什么，不要在我的照片上做一些额外的操作，这种行为很让人讨厌。有点那种到此一游的感觉，自以为很聪明，乱涂乱画，搞得很心烦。

图片质量、图片拍摄日期、GPS等照片里面的原始信息也不要给我乱改动，有时候copy的时候，照片的原始信息可能也会丢掉，比如创建时间、修改时间等一些文件的元信息被修改了，当然对看图片影响不大，但是也让人讨厌，总感觉丢失了些什么。其实也可以说有点吹毛求疵，但是我就是这么追求原汁原味，不失真。

为什么呢？



## *<2020-11-20 五>* ##

### 要对自己表述的逻辑充满信心 ###

对于我们花费大量时间、金钱，学习、实践并最终留于认知的内容，在用于论述的证据时，应该要有十足的信心相信是对的。如果我们都没信心某些方面来说是对的，我们为什么还要花费时间学习，并让错误的东西轻而易举的进入我们的认知？都花费如此多的时间学习了，那肯定大部分是对的而只有一小部分是错误的，那何不尽早删除掉这一小部分错误？如果大部分都是错误的，那这人得有多智障，花费了巨大的成本换来的确实错误的认知。对自己的表述的逻辑有信心，有丰富的工具手段，让自己对自己的认知有清醒的认识。

### base64 encode jpeg images ###

`sed 's/^.\{23\}//g' base64_encoded_jpeg.txt|base64 -d >origin.jpeg`

`key="";redis-cli -n 2 -h m1124-p 11240 get ${key}|sed 's/^.\{23\}//g'|base64 -d >origin.jpeg`


`usercode=;redis-cli -n 2 -h m1 -p 11240 get photo::10000000${key}|sed 's/^.\{23\}//g'|base64 -d >${key}.jpeg`



key=;redis-cli -n 2 -h  -p 11240 get photo::${key}|sed 's/^.\{23\}//g'|base64 -d >${key}.jpeg

key=;redis-cli -n 2 -h m12. -p 11240 get photo::${key}|sed 's/^.\{23\}//g'|base64 -d >${key}.jpeg

key=;redis-cli -n 2 -h m1 -p 11240 get photo::${key}|sed 's/^.\{23\}//g'|base64 -d >${key}.jpeg


## *<2020-10-22 四>* ##

[十年IT灾难全面回顾和总结](https://www.csdn.net/article/2015-12-28/2826562)


什么是好的代码实现？逻辑结构清晰，层次错落有序
逻辑结构：
业务逻辑
模型逻辑
业务-模型适配逻辑



## *<2020-10-16 Fri>* ##

打的一拳开，免得百拳来


## *2019.11.11* ##

ldap 验证用户密码是否正确，需要使用 upn  或者 dn 作为用户名 https://github.com/Adldap2/Adldap2-Laravel/issues/580

## *Sun Sep 29 20:34:46 CST 2019* ##
引用透明性 & 可重入性

[引用透明，最初是个数学概念，表示在同一作用域内，相同表达式的值相同](https://www.zhihu.com/question/52147030/answer/274972772)

[引用透明是指，在作用域内，x是多少，就永远是多少，所有引用x的表达式]( https://www.zhihu.com/question/52147030/answer/129190223)

`如果一个函数的输入相同，对应的计算结果也相同，那么它就具备「引用透明性」`  貌似是可重入性

## *2016.08.08* ##
如果看起来是只鸭子，那就当成一只鸭子对待。

## *2016.07.15* ##
消息队列的本质就是对信息有一对接口可以进行存取beanstalk ,redis 可以做的，mysql当然也可以做，只是效率问题而已


## *2016.07.14* ##
Yii2 `Model` 子类里面定义了和数据库字段同名的公有属性，数据库对应的属性会被覆盖，无法给其赋值，更新。
可以使用 `\Yii::error(VarDumper::dumpAsString($model));` 查看一下对象值，就一目了然也。。


简繁体汉子匹配的正则 `[一-龠]`


## *2016.07.11* tweet 开张了。。。 ##

设计是自己的短板，还是借用别人的使用一下吧，样式抄自于  [http://www.yinwang.org/tweet.html](http://www.yinwang.org/tweet.html) ,并做了一点修改。
