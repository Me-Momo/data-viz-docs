# 子弹图

> 语雀链接：[https://www.yuque.com/wuming-1gzjy/qzthlw/dcn0eq](https://www.yuque.com/wuming-1gzjy/qzthlw/dcn0eq/edit)

## 图表简介
子弹图的发明是为了取代仪表盘上常见的那种里程表，时速表等基于圆形的信息表达方式
1. 线性的表达方式来表达丰富的数据信息，更加合理的利用空间。
1. 从可视化阅读性的角度，子弹图可以更直观的看到**当前进展的具体值和占比**。<br />
1. 从页面布局结构来看，子弹图这类进度条图表使布局更紧凑。

主要使用场景是企业项目目标进度管理和KPI考核，它可以清晰的反映出指标度量的数字变化和完成情况，直观、高效展示数据。了解关注目标是多少，当前进展是到了多少，进展是否正常；还有一些极端情况是进展如果超过目标，这种情况现有仪表盘无法显示。

## 图表详解
### 构成
![image.png](https://cdn.nlark.com/yuque/0/2019/png/221520/1547373003922-201c0554-7c95-46d9-bdf4-960e337f8e32.png#align=left&display=inline&height=170&linkTarget=_blank&name=image.png&originHeight=340&originWidth=1200&size=38796&width=600)
### 说明
**功能度量**分段颜色条形**定性范围**得分。每种色调（如上面示例中三种不同深度的灰色）表示不同表现范围等级，如欠佳、平均和良好。当使用子弹图时，建议最多使用五个等级。

## 图表故事
最常见的一个案例是实际销售量和预计销售量的关系，我们想要传达的关键信息是，实际发生的结果是否达到预期的目标值，以及当前进展属于悲观目标、正常目标还是乐观目标。<br />如下图，蓝色进度代表的是实际数值，背景的三种颜色区间代表完成进度的等级：差、良、优。<br />图表阅读不同于文字阅读，读者往往会聚焦于最显眼的部分。通过下图，很直观的传达了当前的销售总额打破预期目标值，并且属于优秀目标的信息～

![image.png](https://cdn.nlark.com/yuque/0/2019/png/221520/1547374686985-6b23faf1-88dd-4695-94a1-eecf6d1f625c.png#align=left&display=inline&height=98&linkTarget=_blank&name=image.png&originHeight=208&originWidth=1070&size=14445&width=503)<br />还有一种复杂的场景是衡量每个月销售额的完成情况，采用拆分复合子弹图的形式予以呈现,可以对比不同月份之间的目标进展情况

![image.png](https://cdn.nlark.com/yuque/0/2019/png/221520/1547375297090-34ef3ea0-528d-4f4b-972b-189b587ce65c.png#align=left&display=inline&height=203&linkTarget=_blank&name=image.png&originHeight=516&originWidth=1320&size=42775&width=519)

## 可视化作品

![](https://cdn.nlark.com/lark/0/2018/png/46109/1534311382923-c8d7ff99-c697-4ae5-bf1f-60a0802545a4.png#align=left&display=inline&height=218&linkTarget=_blank&originHeight=371&originWidth=1011&width=594)<br />更多请看: [http://datavizproject.com/data-type/bullet-graph/](http://datavizproject.com/data-type/bullet-graph/)

## 图表制作
| BI工具 | Tableau | [https://onlinehelp.tableau.com/current/pro/desktop/en-us/qs_bullet_graphs.htm](https://onlinehelp.tableau.com/current/pro/desktop/en-us/qs_bullet_graphs.htm) |
| :---: | :---: | :--- |
|  | Power BI | [https://powerbi.microsoft.com/en-us/blog/tag/bullet-chart/](https://powerbi.microsoft.com/en-us/blog/tag/bullet-chart/) |
|  | Excel | [http://www.exceluser.com/excel_dashboards/bullet-graph.htm](http://www.exceluser.com/excel_dashboards/bullet-graph.htm) |
|  | 其他 | 略 |
| 可视化库 | AntV | [G2官方实例](https://antv.alipay.com/zh-cn/g2/3.x/demo/other/bullet-graph.html) |
|  |  | 1、G2的官方实例比较耦合数据，所以我提供了一个自定义shape的方式<br />可以看[demo](https://codepen.io/kasmine/pen/dqyLMz?editors=0010)，只需要修改configData就可以了 |
|  |  | 2、G2的官方实例其实还有很多细节没有处理，要使用的话，需要自己好好处理一番 |
|  | powerBI | [https://github.com/Microsoft/powerbi-visuals-bulletchart](https://github.com/Microsoft/powerbi-visuals-bulletchart) |
| 其他 | AnyChart | [https://docs.anychart.com/Basic_Charts/Bullet_Chart](https://docs.anychart.com/Basic_Charts/Bullet_Chart) |
|  | HighChart | [https://www.hcharts.cn/demo/highcharts/bullet-graph/dark-unica](https://www.hcharts.cn/demo/highcharts/bullet-graph/dark-unica) |

## 参考
1. [DataVizProject](https://datavizproject.com/data-type/bullet-graph/)
1. [Bullet Graph - wiki](https://en.wikipedia.org/wiki/Bullet_graph)
