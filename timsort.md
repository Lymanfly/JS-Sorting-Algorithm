# TimSort

TimSort 是一个归并排序做了大量优化的版本。对归并排序排在已经反向排好序的输入时做了特别优化。对已经正向排好序的输入减少回溯。对两种情况混合（一会升序，一会降序）的输入处理比较好。


## 1. 算法步骤

1.扫描数组，确定其中的单调上升段和严格单调下降段，将严格下降段反转；
2.定义最小基本片段长度，短于此的单调片段通过插入排序集中为长于此的段；
3.反复归并一些相邻片段，过程中避免归并长度相差很大的片段，直至整个排序完成，所用分段选择策略可以保证O(n log n)时间复杂性。

## 2. 动图演示

![动图演示](res/TimSort.gif)


## 3. 什么时候最快

当输入的数据已经是正序时（都已经是正序了，我还要你冒泡排序有何用啊）。


## 4. 什么时候最慢

当输入的数据是反序时（写一个 for 循环反序输出数据不就行了，干嘛要用你冒泡排序呢，我是闲的吗）。


## 5. Java 代码实现

```java

```
