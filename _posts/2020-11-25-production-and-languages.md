---
title: "production and languages"
date: 2020-11-25
---

感觉上sql这套东西还是不适合production

简单的查询，小的pipeline，非production的地方可能没问题

但是一旦逻辑变得复杂，比如很多if else，或者很多的business logic，无论是改还是测试都很不方便

传统的c++这种语言还是更适合production，优点有

1. 可以handle复杂的逻辑
2. 封装，复用更加方便
3. 测试方便，工具齐全，有continous integration
4. 执行效率更高
5. 优化起来更方便
6. 并行处理和运行
7. 打包，release，可以follow简单并且标准的流程
8. 跟其他已有的基于c++的系统无缝的连接

当然，如果是非production的东西，sql, python, colab这种东西可能会更适合，优点有

1. 更少的代码
2. 无需编译，即时运行
3. 更快的迭代和反馈
4. 结果可视化
5. 分段运行
6. overhead小
7. 也不需要别人code review

感觉上又回到了很多年前在阿宽公司搞matlab和c的日子。一般上来说，需要两条腿跑路。
