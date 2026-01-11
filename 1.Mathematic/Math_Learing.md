# 第一章 数学知识
___
## 目录
- #### 1.1 指数
- #### 1.2 对数
- #### 1.3 级数
- #### 1.4 模运算
- #### 1.5 证明方法
- #### 1.6 递归简论
- #### 1.7 总结
- #### 1.8 练习
___
## 1.1 指数
下面给出一些基本公式  
$$ 
\begin{eqnarray}
    X^AX^B & = & X^{A+B}  \\
    \frac{X^A}{X^B} & = & X^{A-B} \\ 
    (X^A)^B & = & X^{AB}  \\
    X^N + X^N & = & 2X^N \neq X^{2N} \\ 
    2^N + 2^N & = & 2^{N+1} \\
\end{eqnarray}
$$ 
---
## 1.2 对数
约定俗成地把 $ log_2 $ 记作 $ log $  
有以下几个定理
$$
\begin{eqnarray}
    \log_AB & = & \frac{\log_C{B}}{\log_C{A}} \\
    \log{AB} & = & \log{A} + \log{B} \\
    \log{\frac{A}{B}} & = & \log{A} - \log{B} \\
    \log{A^B} & = & B\log{A} \\
\end{eqnarray}
$$
---
## 1.3 级数
下面先给出两个最基本的公式
$$
\begin{eqnarray}
    \sum_{i=0}^N 2^i & = & 2^{N+1} - 1 \\ 
    \sum_{i=0}^N A^i & = & \frac{A^{N+1} - 1}{A - 1}
\end{eqnarray}
$$
在第二个公式中，若$ 0 < A < 1 $则
$$
    \sum_{i=0}^N A^i \leq \frac{1}{A - 1}
$$  
当且仅当$ N \to \infty $该和趋近于$ \frac{1}{A - 1} $
