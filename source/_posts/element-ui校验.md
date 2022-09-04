---
title: element-ui校验
date: 2022-08-31 21:57:27
tags:
---
>首先需要给表单绑定 :rules="ruleInline" 后面的是校验的对象名

![](./element-ui%E6%A0%A1%E9%AA%8C/1.png)

>在data的return加上一个对象校验规则，校验规则数组模式

![](./element-ui%E6%A0%A1%E9%AA%8C/2.png)

>用prop依次绑定每个表单项
>(注意: 校验数组名必须和V-model绑定的名字一样)

![](./element-ui%E6%A0%A1%E9%AA%8C/3.png)

>这个异步需要些await用于校验是否通过
![](./element-ui%E6%A0%A1%E9%AA%8C/4.png)

>最后关闭的时候清空事件close
![](./element-ui%E6%A0%A1%E9%AA%8C/5.png)

>用于清空校验产生的红色提示关闭后消失
![](./element-ui%E6%A0%A1%E9%AA%8C/6.png)