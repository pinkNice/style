# 现行项目UI介绍

> 项目项目包含以下多个项目：
 
1. 数字包包出版社
2. 学考无纸化考试

两者项目共同点是，都使用了antd框架，故请阅读antd框架API，便于开发.

[antd链接地址:https://antd-mobile.gitee.io/index-cn](https://antd-mobile.gitee.io/index-cn) 


### [数字包出版社项目UI介绍](digitalPackage/readme.md)

> 数字包出版社项目页面如下：
 
1. 数字包已购/未购列表
2. 数字包详情
3. 数字包练习目录
4. 数字包答题
5. 数字包
6. 查看解析

> 数字包答题与查看解析 使用的是教研测项目的UI。


#### 数字包出版社UI架构


##### [core](digitalPackage/core/readme.md)

1. [reset  //重置默认样式](digitalPackage/core/reset.md)			
2. [setting //全局底层变量集合，请谨慎更改](digitalPackage/core/setting.md)
3. [common //全局公用class集合，请谨慎更改](digitalPackage/core/common.md)

##### [components](digitalPackage/components/readme.md)

2. [serach input](digitalPackage/components/search.md)
3. [tab screen](digitalPackage/components/tabScreen.md)
4. [left img and text](digitalPackage/components/imgText.md)
5. [catalog](digitalPackage/components/catalog.md)
6. [pull up refresh](digitalPackage/components/pullUpRefresh.md)
7. [dialog](digitalPackage/components/dialog.md)
8. [null page](digitalPackage/components/null.md)




### [无纸化考试项目UI介绍](noPaperTest/readme.md)

> 无纸化考试项目页面如下：
 
1. 学考题库

		试卷列表

		试卷详情

2. 已购买列表

		试卷答题

3. 查看测评页面

		查看解析

		邀请好友页

4. 错题本

		错题列表

		错题详情

> 无纸化考试答题、查看解析、错题本详情使用的是教研测项目的UI。教研测UI使用了antd框架


#### 无纸化考试UI架构


##### global

1. [index  //重置默认样式 + 全局公用class + 重置antd框架UI](noPaperTest/index.md)			
2. [variables //项目主题，变量集合](noPaperTest/variables.md)




