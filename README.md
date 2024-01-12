## **介绍**
提供一些常见的Python画图示例，更好赶论文

## **解决中文乱码**
[解决方法](https://zhuanlan.zhihu.com/p/566430362)

**使用的时候记得修改为**
```
fig.savefig('./pics/{name}.pdf', format='pdf')
```
这样直接导出pdf插入tex就行了

## 一些链接
[**matplotlib命令与格式：图例legend语法及设置**](https://blog.csdn.net/helunqu2017/article/details/78641290)

[**matplotlib命令与格式：标题(title),标注(annotate),文字说明(text)**](https://blog.csdn.net/helunqu2017/article/details/78659490)

[**这里可以挑 color 和 marker样式**](https://cloud.tencent.com/developer/article/1540478)

[**单行热力图 & 可以挑热力图的颜色**](https://www.codenong.com/cs106384659/)
### 折线图
```
plot_line()
```
![avatar](pics/line.png)

### 柱状图
```
plot_bar()
```
![avatar](pics/bar.png)

### 多柱状图
多组数据展示利器
```
plot_multi_bar()
```
![avatar](pics/multi_bar.png)

### 柱状+折线
有时单条线或单个柱子太单调了
```
plot_bar_and_line()
```
![avatar](pics/bar_and_line.png)

### 散点图
```
plot_scatters()
```
![avatar](pics/scatter.png)

### 热力图
```
plot_hetmap()
```
![avatar](pics/heatmap.png)

### 组合图1
喜欢用来画多个数据集的ablation,当然也可以画成4个小图在tex里拼装，但可能图之前的缝隙会比较大
```
plot_ablation_bar_in_one()
```
![avatar](pics/ablation.png)

### 组合图2
可以用在验证某方法具有泛化性，然后所有模型试一遍。难点在于一个字图省掉横坐标，且上下对齐。（其实我也不知道这样有啥好，嘻嘻）
```
plot_two_bar_in_one()
```
![avatar](pics/two_bars.png)

### 向量可视化
t-SNE可视化，提供的例子是一个画embedding随训练变化的例子
```
draw_tsne.py
```
![avatar](pics/tsne.png)
