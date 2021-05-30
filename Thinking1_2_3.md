### Thinking 1:常见的规划问题都包括哪些？

** LP：线性规划,Linear Programming  研究线性约束条件下线性目标函数的极大或者极小值问题
** ILP： 整数线性规划Integer Linear Programming 全部决策变量必须为整数，而且是离散的
** MIP：混合整数规划,Mixed Integer Programming 混合整数规划是LP的一种，其中部分的决策变量是整数（不要求全部都是整数）
** VRP：Vehicle Routing Problem 车辆路径问题


## Thinking 2：常用的规划工具包都有哪些？
开源的
pulp 只用于线性模型，包括如整数规划、01规划，还是混合整数线性规划

ortools Google开发，用于优化的开源软件 可以解决车辆路径、流程、整数和线性规划等问题, 大厂的开源产品，质量有保证 

商业的
阿里的VRP的产品，只用于内部


Thinking 3：TSP与VRP问题的关系是怎样的？
本质是：1个人多个地点  VS 多个人多个地点
旅行商问题（Traveling Salesman Problem, TSP） 有一个推销员，要到n个城市推销商品，他要找出一个包含所有n个城市的具有最短路程的环路。
多回路运输问题（Vehicle Routing Problem, VRP）对一系列客户的需求点设计适当的路线，使车辆有序地通过它们，
在满足如下的约束条件下:
  货物发送量, 需求量、交货时间、车辆载长宽限制，载荷限制、行驶安全限制等等，
达到一定的优化目标如下：
  里程最优、费用最省、时间最短，用车最少。
VRP是世界级的难题，有巨大的商业价值。