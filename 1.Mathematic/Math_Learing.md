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
当且仅当$ N \to \infty $该和趋近于$ \frac{1}{1 - A} $  
下面进入无穷级数$ \sum_{i=0}^\infty A^i (0 < A < 1) $的结果的推导
$$
\begin{gather}
    令S = \sum_{i=0}^\infty A^i = 1 + A + A^2 + A^3 + ... \\
    则AS = A + A^2 + A^3 + ... \\
    故S - AS = 1,即得到S = \frac{1}{1 - A}
\end{gather}
$$
还有另一种常用的级数是算术级数，任何算术级数都可以通过基本公式计算，例如
$$
\begin{eqnarray}
    \sum_{i=1}^N i & = & \frac{N(N+1)}{2} \approx \frac{N^2}{2} \\
    \sum_{i=1}^N i^2 & = & \frac{N(N+1)(2N+1)}{6} \approx \frac{N^3}{3} \\
    \sum_{i=1}^M i^k & \approx & \frac{N^{k+1}}{\left| {k+1} \right|}
\end{eqnarray}
$$
易知$ k = -1 $时第三个公式不成立。此时我们需要引入数$ H_N $——调和数，其和称为调和和。  
下面近似式中的误差趋近于$ \gamma \approx 0.57721566 $，这个值称作**欧拉常数**
$$ H_N = \sum_{i=1}^N \frac{1}{i} \approx \log_{e} N $$
---
