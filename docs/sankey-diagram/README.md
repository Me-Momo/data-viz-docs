# 桑基图

> 语雀地址: https://www.yuque.com/wuming-1gzjy/qzthlw/egdsp4

## 图表简介
桑基图，是用于描述从一组值到另一组值的流的可视化，它是一种具有多用途的流程图，可以应用于许多不同的领域。当您希望显示两个域（例如，大学和专业）之间的**多对多映射**或通过**一组阶段的多路径**时都可以使用桑基图(例如，Google Analytics使用sankeys来显示网站上流量如何从页面流向其他页面）

**注意: **使用桑基图要注意的是数据要避免环路，下面3种场景图表不会渲染：1. 节点A连接到它本身 2. 节点A连接到节点B，节点B连接节点C，节点C又连接到节点a。

此处的桑基图打破了能量守恒的思想，得以更广的使用

## 图表详解
### 构成
![image.png](https://cdn.nlark.com/yuque/0/2019/png/221520/1547138047459-046c84a1-a7bb-404a-a9b9-5e1b7c88c7c4.png#align=left&display=inline&height=369&linkTarget=_blank&name=image.png&originHeight=738&originWidth=1244&size=74538&width=622)<br />原图地址: [https://antv.alipay.com/zh-cn/vis/chart/sankey.html](https://antv.alipay.com/zh-cn/vis/chart/sankey.html)

### 种类
桑基图的变体很多，下面列举有几个～

* 表格桑基图

![](https://cdn.nlark.com/lark/0/2018/png/46109/1545353125049-65a099ec-817b-45f6-b8ef-6adab0e1e9e1.png#align=left&display=inline&height=122&linkTarget=_blank&originHeight=304&originWidth=1856&width=747)
* 来源去向图

![](https://cdn.nlark.com/lark/0/2018/png/46109/1545353138678-fda8f08a-4a79-44dd-b798-c7935e42e317.png#align=left&display=inline&height=116&linkTarget=_blank&originHeight=286&originWidth=1836&width=747)

* 带回环的桑基图

![](https://cdn.nlark.com/lark/0/2018/png/46109/1545353506206-a55c5b64-3145-4f1f-9f87-efd6db0acf9a.png#align=left&display=inline&height=110&linkTarget=_blank&originHeight=268&originWidth=1814&width=747)

参考：[https://www.sankeyflowshow.com/intro/sankeydiagrams.html](https://www.sankeyflowshow.com/intro/sankeydiagrams.html)

## 图表故事
### 适用场景1：随时间的变化分析或路径分析
假设有4款产品，以下是它四个月内的活跃数据

![](https://cdn.nlark.com/lark/0/2018/png/46109/1545813745672-33d22a25-741e-464a-a1a6-28220dda6feb.png#align=center&display=inline&height=88&linkTarget=_blank&originHeight=196&originWidth=1142&width=514)<br />
<br />这个数据除了看出活跃用户数在上升，沒有任何分析的意义。让我们进一步拆分指标，根据不同活跃用户的使用时间进行拆分，以及引入不活跃用户。因此进行了更全面的指标对比：流失用户、不活跃用户、活跃用户、忠诚用户、回流用户。<br />![](https://cdn.nlark.com/lark/0/2018/png/46109/1545815749994-bee5f682-c67a-4eef-b51f-7ca899f36e63.png#align=center&display=inline&height=231&linkTarget=_blank&originHeight=914&originWidth=1450&width=366)<br />看到上面的表格其实很懵逼，让我们看看桑基图怎样更清晰地表示这些数据。

![](https://cdn.nlark.com/lark/0/2018/png/46109/1545816016905-c397acd1-cf56-4bef-b14c-dae2237889cb.png#align=center&display=inline&height=249&linkTarget=_blank&originHeight=840&originWidth=1402&width=415)

根据上图的可视化，我们可以找到一些关键的分析点：**新增用戶数是否大于流失用戶数，每个月新老用户的转化情况，哪个阶段的用户流失较高等。**基于这些，运营可以针对不同的活跃群体进行深入分析，比如说用户为什么不活跃了，什么样的用户能成为忠诚用戶，什么样的用户会流失？这些深入分析通常是围绕着自己的产品和业务展开的。

### 适用场景2：网站流量分析
存在流失情况<br />![image.png](https://cdn.nlark.com/yuque/0/2019/png/221520/1547137160065-9278e1e0-ed33-43d9-a43a-e93dcbbd24d7.png#align=left&display=inline&height=314&linkTarget=_blank&name=image.png&originHeight=1220&originWidth=2230&size=220317&width=575)<br />地址：[https://www.anychart.com/products/anychart/gallery/Sankey_Diagram/User_Flow_Chart.php](https://www.anychart.com/products/anychart/gallery/Sankey_Diagram/User_Flow_Chart.php)

### 适用场景3：**不同变量之间的多对多关系
![image.png](https://cdn.nlark.com/yuque/0/2019/png/221520/1547137082382-030cadec-c7e7-4517-83df-4f1aded188e7.png#align=left&display=inline&height=300&linkTarget=_blank&name=image.png&originHeight=1310&originWidth=2554&size=603661&width=585)<br />地址：[https://my.infocaptor.com/dash/mt.php?pa=usa_presidents_55e9b4e29e3c7](https://my.infocaptor.com/dash/mt.php?pa=usa_presidents_55e9b4e29e3c7)

### 不适用场景
我们先来看一个简单的例子：

![](https://cdn.nlark.com/lark/0/2018/png/46109/1545348951986-d34a2891-f924-422b-bde2-7b9018f32830.png#align=center&display=inline&height=212&linkTarget=_blank&originHeight=649&originWidth=549&width=179)<br />
<br />现在的图表清楚地显示了一些内容，观察者可以从这种可视化中获取到下面的信息：
* **技术**销售量最大**的产品类别
* **南方**销售量最小**的区域 - 其他区域的销售量类推 

然后？似乎感觉大多数洞察来自可视化两侧的条形图 - 而不是实际的“流动”（这又是误导性的吗？）<br />那我们再考虑看下，单纯使用条形图来展示上面的情况：

![](https://cdn.nlark.com/lark/0/2018/png/46109/1545349948085-56048344-d18b-4006-b37a-e3baa34a73b5.png#align=center&display=inline&height=145&linkTarget=_blank&originHeight=145&originWidth=640&width=640)<br />各地区不同产品类型的销售情况<br />我们可以看到，**办公产品无论在哪个地区，销售情况都是最差的**。如果我们想要进一步进行跨区域的比较，那该怎么办？这个时候，我们进行维度的切换，如下：

![](https://cdn.nlark.com/lark/0/2018/png/46109/1545350056162-24830500-3faf-44dd-9c8a-01ddca03b7d7.png#align=center&display=inline&height=165&linkTarget=_blank&originHeight=165&originWidth=608&width=608)<br />我们现在可以看到**南部地区在各个产品类别的销售情况都不佳**，**西部地区在办公用品方面特别差**。 这两个条形图都显示了我们无法从Sankey获得的额外见解。<br />[原文地址](https://sciolisticramblings.wordpress.com/2018/11/23/sankey-charts-the-new-pie-chart/)
#### [](https://yuque.antfin-inc.com/st5m2s/qmoctl/gk847q#2xtgsv)总结
**「并没有糟糕的图表，糟糕的是选择了错误的图表」**<br />总结下来有两个原则：
1. 解释性可视化：故事在解释性可视化中，是否可以成功传达您要讲述的故事
1. 探索性可视化：如果可视化是探索性的，那么花点时间看一下可视化，可以获取到什么内容？

注意：如果是想通过直观的可视化方式传达数据中的信息给他人（可能会是静态图表的展示方式），这个时候，要判断下您的可视化是否有效，有没有更简单的图表方案来帮助您讲述故事和传达信息。

## 可视化作品
略

## 图表制作
| BI工具 | Tableau | [https://www.youtube.com/watch?v=1HwCzlA9hI4](https://www.youtube.com/watch?v=1HwCzlA9hI4) |
| :---: | :---: | :--- |
|  |  | 制作比较麻烦，需要30分钟以上  |
|  | Power BI | [https://powerbi.microsoft.com/en-us/blog/visual-awesomeness-unlocked-sankey-diagram/](https://powerbi.microsoft.com/en-us/blog/visual-awesomeness-unlocked-sankey-diagram/) |
|  |  | PowerBI的桑基图结点拖拽后,位置信息可保存 |
|  | 其他 | SmartBI、[BDP](https://me.bdp.cn/index.html#/dash_edit/proj_b1a80948a07eddb103cf4d4d25c7a6a3/dsh_5f1cb0939947a042e95b61efffd2b58d)等 |
| 可视化库 | ECharts | [官方实例](http://echarts.baidu.com/examples/#chart-type-sankey) |
|  |  | 还有所欠缺，比如无法设置层级，<br />第一层级的结点不支持存在流失情况 |
|  | AntV | [G2官方实例](https://antv.alipay.com/zh-cn/g2/3.x/demo/relation/sankey-layouts.html)<br />[G6官方实例](https://antv.alipay.com/zh-cn/g6/2.x/demo/flow/table-sankey.html) |
|  |  | AntV实现的桑基图版本，交互效果都比较差 |
|  | powerBI | [https://github.com/Microsoft/powerbi-visuals-sankey](https://github.com/Microsoft/powerbi-visuals-sankey) |
|  | D3 | [http://bl.ocks.org/emeeks/1dd092dadc02a93cdebc](http://bl.ocks.org/emeeks/1dd092dadc02a93cdebc) |
| 其他 | amcharts | [https://www.amcharts.com/demos/sankey-diagram/](https://www.amcharts.com/demos/sankey-diagram/) |
|  |  | 结点有交互，点击后可以收起 连接 |
|  | AnyChart | [https://docs.anychart.com/Basic_Charts/Sankey_Diagram](https://docs.anychart.com/Basic_Charts/Sankey_Diagram) |
|  | Vizlib | [https://www.vizlib.com/sankey/](https://www.vizlib.com/sankey/) |
|  | ifu | [https://www.ifu.com/en/e-sankey/features/](https://www.ifu.com/en/e-sankey/features/) |

## 参考
1. [员工流量桑基图](https://zhuanlan.zhihu.com/p/26193967)
1. [BDP社区对于桑基图的介绍](https://bbs.bdp.cn/thread-141-1-1.html)
1. [Sankey Diagram Drawing Tools]() 👍

