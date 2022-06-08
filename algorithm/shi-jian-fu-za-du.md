# 时间复杂度

## 东东的文章 最靠谱的最细致的讲解

[https://mp.weixin.qq.com/s/OQAzopRncZe5cb9\_of4mCQ](https://mp.weixin.qq.com/s/OQAzopRncZe5cb9\_of4mCQ)

递归算法的时间复杂度 = 递归的次数 x 函数本身的时间复杂度

递归算法的空间复杂度 = 递归堆栈的深度 + 算法申请的存储空间

或者再说得直观一点：

递归算法的时间复杂度 = 递归树的节点个数 x 每个节点的时间复杂度

递归算法的空间复杂度 = 递归树的高度 + 算法申请的存储空间

## For DP

\
\#暴力解 \
时间复杂度：O(K^N) \* O(K) = O(K^(N+1))\
空间复杂度：O(N)

\#对于 **带备忘录** 的动态规划算法的**时间复杂度**，以下几种理解方式都是等价的： \
&#x20;   \
递归的次数 x 函数本身的时间复杂度 \
\= 递归树节点个数 x 每个节点的时间复杂度 \
\= 状态个数 x 计算每个状态的时间复杂度 \
\= 子问题个数 x 解决每个子问题的时间复杂度 \
\= O(N) \* O(K) = O(NK)

\#**备忘录优化** 解法的**空间复杂度** \
\
dp函数的堆栈深度为「状态」的个数，依然是O(N)\
而算法申请了一个大小为O(N)的备忘录memo数组，所以总的空间复杂度为O(N) + O(N) = O(N)。

## For 回溯算法

**时间复杂度**：\
递归的次数 x 函数本身的时间复杂度 \
\= 递归树节点个数 x 每个节点的时间复杂度 \
\= O(2^N) \* O(N) = O(N\*2^N)

**空间复杂度**：\
O(N\*2^N)   【O(n) is the height of the tree】

## 三个原则

1.只关注循环执行次数最多的一段代码

2.加法法则：总复杂度等于量级最大的那段代码的复杂度。

3.乘法法则：嵌套代码的复杂度等于嵌套内外代码复杂度的乘积

## [常见时间复杂度曲线](https://juejin.cn/post/6844903750985842695)

![
](../.gitbook/assets/timegraph.jpg)

![更多细节的版本](https://liam.page/uploads/images/Linux/big\_O\_chart.png)

## 1.数据结构

![](https://img-blog.csdnimg.cn/20200813093903438.png?x-oss-process=image/watermark,type\_ZmFuZ3poZW5naGVpdGk,shadow\_10,text\_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80MTg4NDgwOA==,size\_16,color\_FFFFFF,t\_70#pic\_center)

## 2.图

![](https://img-blog.csdnimg.cn/2020081309404930.png#pic\_center)

## 3.排序算法

![](https://img-blog.csdnimg.cn/20200813094157101.png?x-oss-process=image/watermark,type\_ZmFuZ3poZW5naGVpdGk,shadow\_10,text\_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80MTg4NDgwOA==,size\_16,color\_FFFFFF,t\_70#pic\_center)

## 4.搜索算法![](https://liam.page/uploads/images/Linux/big\_O\_chart.png)

![](https://img-blog.csdnimg.cn/20200813094239981.png?x-oss-process=image/watermark,type\_ZmFuZ3poZW5naGVpdGk,shadow\_10,text\_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80MTg4NDgwOA==,size\_16,color\_FFFFFF,t\_70#pic\_center)
