好好起名(Name)
========

### 写在开头

这是为了我的宝宝起名写的程序，宝宝小名好好。

本程序适用于起名三个字的，并且姓氏是单字的情况。

### 开发背景

目前市面上好多都是收费的，而且起的名字还不是相当的好，读起来各种问题，所以还不如自己写个程序来算。

更重要的是，以后别人问我的孩子名字怎么起的，希望孩子很自豪地回答：我爸爸写程序算出来的。

### 运行方式
环境要求python3.6

1.手动配置config.py文件的设置项，比如姓氏、出生时间

2.执行`python main.py`运行程序，看输出日志，初始化数据后这次运行Ctrl+C终止。

3.注意"综合计算的结果"开头的这行结果，记下组合中出现的笔画数字。
```
综合计算的结果： 2 [(3, 15, '土金金', '大吉'), (11, 7, '土土金', '大吉')]
```

4.从`data/full_wuxing_dict.py`挑选第3步骤中笔画的字，填写到`data/self_wuxing_dict.py`文件中的金木水火土对应的位置。比如上面的例子，则选填笔画为3/7/11/15的字。
```
原作者这里写的不太清楚，它是指：
· 如(3, 15, '土金金', '大吉')。
· 意为名字为3个字，姓属「土」，后面名的2个字分别属「金」。
· 于是你需要从 full_wuxing_dict.py 这个文件，找到「金」中的笔划为3、15的两部分（数组），填写到 self_wuxing_dict.py 对应的（五行）位置。
· 之后再从 self_wuxing_dict.py 里筛选名字要的字。
```

5.再次执行`python main.py`运行程序，喝杯咖啡后再回来看name.txt文件的结果吧。

### 参考起名的方法：

* 三才五格
* 喜用神
* 易经五行
* 百家姓最佳搭配
* 老婆私人订制
* 单个名确认后再起名

#### 结语
代码完全开放公开，如果有用，请点下Star表示支持。
