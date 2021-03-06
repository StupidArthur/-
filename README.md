# 图论基本算法
**2020-7-19**
***
### 二分图
> 一个图的所有顶点可以划分成两个子集，使得所有边的出度和入度顶点分别在这两个子集中。

**BFS染色法**
只用黑白两种颜色，能不能使每个点都染上色，并且相邻的两点点色不同

**二分图最大匹配**
满足二分图的最大边数
**交替路** - 从一个未匹配的点出发，一次经过未匹配边、匹配边、未匹配边...这样的通路。
**增广路** - 从一个未匹配的点出发，走 **交替路** 到达了一个未匹配过的点这样的通路。
**匈牙利算法** - 寻找增广路求出最大匹配数。
**增广路有以下特点**
> 增广路有奇数条边
> 路径上的点一定是一个在X边，一个在Y边，交错出现
> 起点和终点都是目前还没有配对的点
> 未匹配的边数量比匹配边的数量多1

