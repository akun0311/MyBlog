[TOC]



# 第一章 函数 极限 连续

# 一. 高数基础补充

## 1. 数集

1. 数集就是我们常用的符号

2. 实数集$R=(-\infty, +\infty)$

   ​	注意负无穷和正无穷就是一个**符号**, 而不是一个确切的数

   ​	虽然我们更多的是把它们看作一个数, 但它们确实不是一个数, 它们更像是一个动态的变化

   ​	由于正无穷或者负无穷是一个符号, 而不是一个数, 那么也就意味着我们不可能取到正无穷或者负无穷

   ​	因此正无穷和负无穷只有开区间, 而没有闭区间

3. 正实数$R^{+}=(0, +\infty)$

4. 有理数$Q$: 有理数$Q$其实就是分数形式

5. 整数$Z=\{\cdots, -n, \cdots, -1, 0, 1, \cdots, n, \cdots\}$

6. 正整数$N^{+}=\{1, 2, 3, \cdots,n, \cdots\}$, 正整数不带0

7. 自然数$N=\{0, 1, 2, \cdots, n, \cdots\}$, 自然数带有0


## 2. 区间

1. $(a, b) = \{x| a < x < b\} $

2. $[a, b) = \{x| a \leqslant x < b\} $

3. $(a, b] = \{x| a < x \leqslant b\} $

4. $[a, b] = \{x| a  \leqslant x  \leqslant b\} $**这个叫做有界区间**

5. $(a, +\infty) = \{x| a < x < +\infty\}$

6. $[a, +\infty) = \{x| a \leqslant x <+\infty\}$

7. $(-\infty, b) = \{x| -\infty < x < b\}$

8. $(-\infty, b] = \{x| -\infty < x \leqslant b\}$

9. $(-\infty, +\infty) = \{x| -\infty < x < +\infty\}$**这个叫做实数域**

10. 区间的注意事项

    1. 区间中的x如果没有说明范围的话,x一般都为实数
    2. 无穷只能是开区间, 不能是闭区间, 因为无穷是一个动态的变化, 而不是一个确切的数
    3. $[a, b]$叫做**有界区间**
    4. $(-\infty, +\infty)$**叫做实数域**


## 3. 邻域

1. 邻域本质上指的是就是一个小的**开区间**

   区间内包含$x_{0}$点的叫做**邻域**

   区间内包含$x_{0}$点的叫做**去心邻域**

2. $x_{0}的邻域: U_{\delta}(x_{0})=\{ x|\; |x-x_{0}|< \delta, \delta > 0\}$

3. $x_{0}的去心邻域: U_{\delta}(x_{0})=\{ x|\; 0<|x-x_{0}|< \delta, \delta > 0\}$

## 4. 映射

1. 映射的分类(x和y的对应关系)
   1. 一对一映射
   2. 多对一映射
   3. 一对多映射
   4. 多对多映射(乱射)

2. 映射分类示意图

   ​	![image-20230310230710001](C:\Users\29698\Desktop\高数笔记\imgs\image-20230310230710001.png)

# 二. 函数

## 1. 函数的概念

1. **函数的定义:** 对于$f=dx$, 且$x \in D,y\in R, 其中每一个x都有一个唯一的y与之对应$

   ​	$x\in D$, 称D为定义域 

   ​	$y \in R$, 称R为值域

2. **函数的两要素<1定义域. 2映射法则>**

   1. 函数的定义域和映射法则能够确定一个唯一的函数

      当两个函数的定义域和映射法则相同的时候, 这两个是相同的函数

      当两个函数的定义域和映射法则不同的时候, 这两个函数不同

   2. 函数的两要素当中没有值域的原因是因为, 当我们有了定义域和映射法则之后, 我们就可以确定函数的值域了

3. **函数注意事项**

   1. 函数和自变量的符号无关, 函数的两要素是定义域和映射法则, 因此函数只与定义域和映射法则有关系

   2. 当求函数的定义域的时候, 不能先化简函数, 我们需要先求完定义域,然后再化简函数

## 2 .常见的函数

### 1. 初等函数

1. **常值函数 $y=c$**

   注意常值函数的奇偶性判断: $(在c !=0的时候是偶函数, 在c==0的时候既是奇函数也是偶函数)$

2. **幂函数: $y=x^{u}$**

   幂函数都过定点$(1, 1)$, 函数的曲线在$u>1$时抬头, $u<1$时低头

3. **指数函数: $ y=a^{x}$** 

   1. 指数函数都过定点$(0,1)$, 函数的曲线在$a>1$时抬头, 在$a<1$时低头
   2. **指数函数相关性质**
      1. $a^{m} * a^{n} = a^{m+n}$
      2. $\frac {a^{m}}  {a^{n}} = a^{m-n}$
      3. $(a^M)^{N}= a^{M} *a^{M}*a^{M}* \cdots *a^{M} = a^{MN}$
      4. $注意: a^{m^{N}} \neq (a^{m})^{N}, a^{m^{N}} = a^{^{(m^{n})}}$
      5. **指数差**: $e^a-e^b = e^b(e^{a-b} - 1)$

4. **对数函数: $y = \log_{a}x, (a>0, a!=1)$**

   1. 对数函数都过定点$(1, 0)$, 函数的曲线在$a>1$时抬头, $a<1$时低头
   2. 对数函数相关性质
      1. $\log_{a}M + \log_{a}N=log_{a}MN$
      2. $\log_{a}M - \log_{a}N=log_{a} \frac M N$
      3. $\log_{a}M^{N} = N * \log_{a}M$
      4. $\log_{a}\frac 1 M = \log_{a}M^{-1}=-\log_{a}M$
      5. $a^b = e^{\ln a * b}$ **这个是幂指转换公式**
      6. $\log_{a}b= \frac{\log_{c}b}{\log_{c}a}$, **这个是对数换底公式**

5. **三角函数**

   1. $正弦函数y=\sin x$

      ​	$定义域x\in (-\infty, + \infty), 值域y\in[-1, 1], 周期T=2\pi$

   2. $余弦函数y=\cos x$

      ​	$定义域x\in (-\infty, + \infty), 值域y\in[-1, 1], 周期T=2\pi$

   3. $正切函数y=\tan x$

      $定义域 x\neq k\pi + \frac{\pi}{2}, k = 0, +1, -1, +2, -2, \cdots R\in[-\infty,+\infty], 周期T=\pi$

   4. 三角函数的性质
      1.  $\sin^{2}x + \cos^{2}x = 1$
      2.  $\tan^{2}x+ 1 = \sec^{2}x$

6. **反三角函数**

   1. $y = \arcsin x$ 没有周期

      ​	![image-20230311001023171](C:\Users\29698\Desktop\高数笔记\imgs\image-20230311001023171.png)

   2. $y =\arccos x$  没有周期

      ​	![image-20230311001034175](C:\Users\29698\Desktop\高数笔记\imgs\image-20230311001034175.png)

   3. $y = \arctan x$​没有周期

   1. $定义域x\in(-\infty, +\infty), 值域y\in(-\frac {\pi}{2}, \frac {\pi}{2})$
      
   1. 注意$y=\arctan x$的值域是开区间, 并且没有周期
      2. $(\arctan x)' = \frac 1 {1 + x^2} = 1-x^2 + x^4 - x^6+ x^8 + \cdots$
      3. $\arctan x = x-\frac 1 3 x^3 + o(x^3)$

### 2. 复合函数

1. $如果y=f(u) , 且u=g(x), 那么可以推出y=f(g(x)) \\注意g(x)的值域和f(u)的定义域的交集要非空(了解一下就好, 考试不在这里设坑)$
2. 复合函数一般就考复合函数的表达式

### 3. 反函数

1. 反函数之间一般关于$y=x$对称, 一般来说反函数就是值域和定义域互相交换

2. $y= f(x) \left\{ \begin{array}{cols} x=g(y)&与y=f(x)重合\\y=g(x)&与y=f(x)关于y=x对称\end{array} \right.$ 

3. **反函数有两种形式, 因为反函数一般喜欢交换自变量的形式**

   1. 区分这两种形式的方式是使用自变量区分

      自变量是y的, 那么它就和原来函数重合的

      自变量是x的, 那么它就和原来的函数对称

   2. 不过考试的时候不会搞混, 因为考试的时候不会在这里设坑, 所以只需要注意反函数的自变量就可以了

4. 求反函数的步骤

   1. $x=g(y)$
   2. $y=g(x)$
   3. $求y=g(x)的定义->y=f(x)的值域$

### 4. 其他的函数(非初等函数)

1. **绝对值函数**

    ​	$$ y = |x| = \left\{ \begin{array}{rcl} x, &x>0  \\0,& x = 0 \\ -x, & x < 0\end{array} \right.$$

2. **符号函数(工程上用的比较多)**

    ​	$y=sgn x = \left\{ \begin{array}{rcl} 1, & x >0\\0 ,& x=0\\ -1, &x<0 \end{array}\right.$

3. **取整函数 $y=[x]$, 其中$[x]$表示不大于x的最大整数**

   ​	![image-20230311095147471](./imgs/image-20230311095147471.png)

4. **狄利克雷函数**

    ​	$$ D(x) = \left\{\begin{array}{cols} 1, &x\in Q \\0, &x\in R/Q \end{array} \right.$$

    1. 这个函数的图像看着是一条直线, 但是如果放大看,就是无穷多的点

    2. 在有界区域上这个函数的定积分是不存在的

       

## 3. 函数的性质

### 1. 奇偶性

1. 函数存在奇偶的前置条件是**函数的定义域D**关于原点$o(0, 0)$对称

    ​	**奇函数**: $f(x) + f(-x) = 0$ , 函数的图像关于原点$o(0, 0)$对称

    ​	**偶函数**: $f(x) = f(-x)$, 函数的图像关于y轴对称
4. **奇偶性需要掌握两点**
   
   1. 判断函数的奇偶性
   2. 掌握一些常见的奇偶函数的性质
5. **判断函数奇偶性的方法**
   1. 先判断定义域是否关于原点$o(0,0)$对称
   2. 然后再验证函数是奇函数还是偶函数
6. **奇偶函数的一些性质**
   	1. $奇*奇=偶: x*x^3 = x^4$
    2. $奇*偶=奇: x* x^2= x^3$
    3. $偶 * 偶 = 偶: x^2 * x^4 = x^6$
    4. $奇+奇=奇$
    5. $偶+偶= 偶$
    6. $偶+奇=?不确定$

7. **奇偶函数的可导性质**
   
   1. $F(x)是可导奇函数, 对于F^{'}(x) = f(x), 则f(x)是偶函数\\比如F(x) = \sin x, f(x) = \cos x$ 
   2. $F(x)是可导偶函数, 对于F^{'}(x) = f(x), 则f(x)是奇函数\\比如F(x) = \cos x, f(x) = \sin x$ 
   3. $f(x)是奇函数, 那么F(x) ={\int_{a}^{x} f(t) \,dt} 是偶函数 $
   4. $f(x)是偶函数, 那么F(x)={\int_{0}^{x}f(t) \,dt }是奇函数$

### 2. 单调性

1. **函数的单调性(以单调增举例)**	
   	$当x_{1} < x_{2}时, \\如果f(x_{1}) < f(x_{2}), 那么称f(x)是单调增的, 此时f^{'}(x)>0. \\如果f(x_{1}) \leqslant f(x_{2}), 那么称f(x)是单调不减的(也可以说成单调增), 此时f^{'}(x)\geqslant 0$	

2. **函数的单调性注意事项**

   1. 函数$f(x)$的单调性一般可以通过一阶导数来判断

   2. 函数的单调性与给定的区间有关, 

      一般而言, 研究函数单调性的时候要指明函数的单调区间

      如果没有明显的指明单调区间, 那么会默认为整个定义域

### 3. 有界性

1. **函数的有界性就是函数有上界或者函数有下界**

2. 函数有界的条件

   ​	$f(x)的定义域是D, 数集X \subset D \\对于任意的x \in X, 存在f(x) \leqslant M, 则说明f(x)有上界\\对于任意的x \in X,存在f(x) \geqslant M, 则说明f(x)有下界 \\对于任意的x \in X, 存在m\leqslant f(x) \leqslant M, 则说明f(x)有界(有上界和下界)$

3. 有界性的一条性质: 有界闭区间上的连续函数必有界

   $f(x)在[a, b]上连续, 则说明f(x)在[a, b]上有界$	

4. **无界的函数就是没有界限, 就是趋于无穷**

### 4. 周期性

1. $对于f(x+T) = f(x), 称T为f(x)的周期\,\,(T>0) \\若存在最小正数T, 则称T为最小正周期$

2. 周期性的注意事项

   1. 周期性主要体现在三角函数上面, 并且一般要求周期T>0

   2. 常值函数$y=c$可以以任何数为周期, 因此它没有最小正周期数T



# 三. 极限

 ## 1. 关于极限的说明

1. **极限的本质就是变化趋势**

   函数极限是函数曲线的变化趋势

   数列的极限就是数列的变化趋势

   但是变化趋势这一名词不太严谨,而数学上的定义需要严谨化和严密化, 才能更好的研究, 因此就有了极限这一词

2. 不能局部取极限





## 2. 数列极限

### 1. 数列极限的概念

 1. **数列极限的相关概念和定义**

    	1. 数列极限指的就是数列的变化趋势$1, \frac 12,\frac 13, \cdots, \frac 1n, \cdots$
     	2. 理解版: 当$n$充分大时, $x_{n}$充分靠近一个数$a$, 数列极限就是$x_{n}$离$a$越来越近

    ​	3. 正式版: 对于任意的$\epsilon>0, 存在一个N, 使得n>N时, |x_{n}-a| < \epsilon成立$

 2. **数列的一般分类**

    1. 数列趋向于某一个值, 此时数列有极限, 如: $1, \frac 1 2, \frac 13, \cdots, \frac 1n, \cdots$
    2. 数列有振荡的现象, 此时数列没有极限, 如: $1, -1, 1, -1,\cdots, (-1)^{n-1}, \cdots $
    3. 数列趋向于无穷, 此时数列没有极限, 如: $1, 2, 3, \cdots, n, \cdots$

3. **数列极限的总结**

   ​	数列存在极限只有一种情况, 就是这个数列趋于一个确定的数, 因此极限必有界(数列收敛)

   ​	而存在振荡和无穷的数列都不存在极限

4. **数列极限存在的充分必要条件: 奇数项和偶数项的极限都存在且相等(都为a)**

   因为数列只有奇数项和偶数项, 除此之外就没有别的了

   $\lim\limits_{n\rightarrow\infty} x_{n} = a \Longleftrightarrow \lim\limits_{n\rightarrow\infty}x_{2n} = \lim\limits_{n\rightarrow\infty} x_{2n-1} = a  $

   ![image-20230306114050057](C:\Users\29698\Desktop\高数笔记\imgs\image-20230306114050057.png)

   

### 2. 数列极限的性质

1. **唯一性**: 如果数列的极限存在, 或者数列收敛的话, 那么数列的极限唯一

   ​	如果极限不唯一的话, 那么就没有办法研究极限了, 东一个西一个的,就乱了.

2. **有界性**: 如果数列的极限存在, 那么数列必有界(有上界或者有下界)

3. **保号性**: 近朱者赤近墨者黑, 数列靠近a, 那么a的性质数列也得有

   1. $\lim\limits_{n\rightarrow\infty} x_{n}=a >0\Longrightarrow 存在一个充分大的n, 使得x_{n}>0 $

   2. $x_{n}> a \Longrightarrow  \lim\limits_{n\rightarrow\infty} x_{n} \geqslant a$

   ​	示例$\frac 1 n > 0 \Longrightarrow \lim\limits_{n\rightarrow\infty} \frac 1n \geqslant0$


### 3. 数列和的极限(重要)

1. ​	![image-20230306153540537](C:\Users\29698\Desktop\高数笔记\imgs\image-20230306153540537.png)

### 4. 求数列极限的方法

#### 1. 夹逼准则

1. 夹逼准则的定义

   ​	$如果y_{n} \leqslant x_{n} \leqslant z_{n}且\lim\limits_{n\rightarrow\infty} y_{n} = \lim\limits_{n\rightarrow\infty} z_{n} = a \\那么\lim\limits_{n\rightarrow\infty} x_{n} = a$

2. 夹逼准则使用建议

   1. 夹逼准则一般用来解一些**有限项求和**的题目, 通常分子分母都带有开方

   2. 如果需要使用夹逼准则解题, 那么使用方法是: 分子不变, 放缩两端的分母
   3. 如果夹逼准则失效, 那么使用定积分定义来解题

   ![image-20230306154216535](C:\Users\29698\Desktop\高数笔记\imgs\image-20230306154216535.png)

   ![image-20230306160120370](C:\Users\29698\Desktop\高数笔记\imgs\image-20230306160120370.png)

   

#### 2. 定积分定义(暂不管)

1. 定积分定义

   ![image-20230306160404741](C:\Users\29698\Desktop\高数笔记\imgs\image-20230306160404741.png)

2. 数列极限和定积分转换的示例	![image-20230306160725737](C:\Users\29698\Desktop\高数笔记\imgs\image-20230306160725737.png)

#### 3. 单调有界原理

1. **单调有界原理的概念和定义**

   $如果数列{x_{n}}满足 (1)x_{n} < x_{n+1}和(2)x_{n}<M, 那么\{x_{n}\}必收敛, 即\lim\limits_{n\rightarrow\infty} x_{n}=A\\注意A是一个确定的, 有限的数$
   
   单调增有上界的数列必有极限
   
   单调减有下界的数列必有极限
   
2. **使用单调有界性原理的解题步骤**

   1. 证明数列有界
2. 证明数列单调
   3. 求出数列的这个极限
   4. 总的来说就是有界, 单调, 求极限
   
3. **使用单调有界原理时的常见不等式**(考试的时候可以直接使用)

   1. $a^2+b^2 \geqslant 2ab$
   2. $a+\frac 1a \geqslant 2(a>0)$
   3. $\sqrt{ab} \leqslant \frac {a+b}{2} $
   4. $x>\sin x \;(x>0)$
   5. $x>ln(1+x) \;\;(x>0)$

#### 4. 归纳法证明数列极限

​		单调有界性原理的题目也可以使用归纳法证明



## 3. 函数极限

### 1. 函数极限的概念

1. 函数极限的概念和定义: 函数极限的本质就是函数曲线的变化取值

2. **函数极限的注意事项**

   1. 函数极限的定义是一个去心邻域, 此时$x\rightarrow{x_{0}}, 但是x 永远取不到x_{0}$
   2. 函数的极限与函数在$x_{0}$处的取值无关, 
   3. 注意函数的极限与函数的表达式和自变量的变化范围有关, 两者缺一不可

3. **函数极限存在的充分必要条件(定理)**

   ​	如果函数存在极限(假设极限值为A),那么函数的左极限和右极限都存在, 且极限值相等(极限值都为A)

   ​	$\lim\limits_{n\rightarrow x_{0}}f(x) = A \Longleftrightarrow \lim\limits_{n\rightarrow x_{0}^+}f(x) =\lim\limits_{n\rightarrow x_{0}^-}f(x) = A$

4. **函数的左极限和右极限**

    1. $函数的右极限: \lim\limits_{n\rightarrow x_{0}^+}f(x) = f(x_{0}-o)=A$
    2. $函数的左极限: \lim\limits_{n\rightarrow x_{0}^-}f(x) = f(x_{0}+o)= A$

5. **$函数f(x)在无穷处(x \rightarrow \infty)的极限$**

   $\lim\limits_{n\rightarrow \infty}f(x) = A,可以记作f(\infty)=A (其中\infty = +\infty 或者-\infty)$

   $由于无穷本质上不是一个数, 而是一个动态的变化$

   $所以函数f(x)在x \rightarrow \infty处的极限是函数在x\rightarrow\infty处的变化趋势$

   $\lim\limits_{n\rightarrow +\infty}f(x) = A, 记作f(+\infty)= A$

   $\lim\limits_{n\rightarrow -\infty}f(x) = A, 记作f(-\infty)= A$	

### 2. 函数极限的性质(待补充)

### 3. 求函数极限方法

#### 1. 两个重要极限

 1. **第一个重要极限**: $\lim\limits_{n\rightarrow 0} \frac {\sin x}{x} = 1$(使用三角函数图求出的)

    1. 衍生的极限:  $\lim\limits_{n\rightarrow \infty} \frac {\sin x} {x} = 0$

    2. $\sin x < x < \frac {\sin x} {\cos x} \Longrightarrow 1 < \frac {x}{\sin x } < \frac {1} { \cos x}$

2. **第二个重要极限**: $\lim\limits_{n\rightarrow \infty} (1+\frac 1 n)^n = e, 注意m,n一般指整数$

    1. 这个极限的极限值等于e的原因是$a_{n} = (1+\frac 1n)^n \;\;其中a_{1}=2, a_{2} = \frac 9 4, a_{3}=\frac {64} {27}$

       可以观察得出$a_{n}$是单调递增的且有上界的, 因此$\lim\limits_{n\rightarrow \infty} (1+\frac 1 n)^n = e$
    注意这个极限的底数和指数是同时变化的
   
2. **这个极限的变形**
   
   ​	$\lim\limits_{n\rightarrow \infty} (1+\frac 1 x)^x = e\\\lim\limits_{n\rightarrow \infty} (1+x)^{\frac 1x} = e$
   
3. **这个极限的本质**
   
   $\lim\limits_{n\rightarrow \infty} (1+无穷小)^{无穷大} = e$
   

![image-20230311151546239](imgs/image-20230311151546239.png)

4. **这个极限的使用示例**
   

​	![image-20230311151847920](imgs/image-20230311151847920.png)



#### 2. 幂指函数转换

1. 幂指函数转换是求函数极限时的一个重要方法

2. 幂指函数转换

   1. $f(x)^{g(x)} = e^{ g(x) *\ln f(x) } $
   2. $g(x)*\ln f(x) = g(x)* \ln f(x) *\ln e$  

3. **幂指函数转换的证明方法**

   ​	$假设\ln f(x) = a, 那么f(x)=e^{a} \\由于a = \ln f(x)(原本的式子) \\因此f(x)= e^{\ln f(x)}\\所以f(x)^{g(x) }=(e^{ \ln f(x)}) ^{g(x)} \\又因为(a^M)^{N}= a^{M} *a^{M}*a^{M}* \cdots *a^{M} = a^{MN} \\所以f(x)^{g(x)} = e^{ g(x) *\ln f(x) }$



#### 3. 函数极限四则运算 

1. 函数极限四则运算的前提条件是 $f(x)和g(x)的极限都存在, 且分母不为0$

   $即\lim\limits_{x\rightarrow x_{0}} f(x)= A且\lim\limits_{x\rightarrow x_{0}}g(x) = B$

2. 加法减法运算

    	1. $\lim\limits_{x\rightarrow x_{0}} (f(x)+g(x))= \lim\limits_{x\rightarrow x_{0}} f(x)+\lim\limits_{x\rightarrow x_{0}} g(x)$
        	2. $\lim\limits_{x\rightarrow x_{0}} (f(x)-g(x)) =\lim\limits_{x\rightarrow x_{0}} f(x) - \lim\limits_{x\rightarrow x_{0}} g(x) $

2. 乘法运算

   ​	$\lim\limits_{x\rightarrow x_{0}} (f(x)*g(x))= \lim\limits_{x\rightarrow x_{0}} f(x)*\lim\limits_{x\rightarrow x_{0}} g(x)$

3. 除法运算

   ​	$\lim\limits_{x\rightarrow x_{0}} \frac {f(x)} {g(x)}= \frac {\lim\limits_{x\rightarrow x_{0}} f(x)} {\lim\limits_{x\rightarrow x_{0}} g(x)} (B \neq 0)$

#### 4. 等价无穷小

1. $如果\lim\limits_{x\rightarrow x_{0}} \alpha(x)= 0且\lim\limits_{x\rightarrow x_{0}} \beta(x), 且\alpha(x) \thicksim \beta(x) $
   $则\lim\limits_{x\rightarrow x_{0}} \frac {\alpha(x)}{\beta(x)} = \lim\limits_{x\rightarrow x_{0}} \frac {\alpha(x)}{\widetilde{\alpha(x)}} *\frac {\widetilde{\alpha(x)}}{\widetilde{\beta(x)}} *\frac {\widetilde{\alpha(x)}}{\beta(x)} =\lim\limits_{x\rightarrow x_{0}} 1 *\frac {\widetilde{\alpha(x)}}{\widetilde{\beta(x)}}  * 1 =  \lim\limits_{x\rightarrow x_{0}}\frac {\widetilde{\alpha(x)}}{\widetilde{\beta(x)}}$
2. 四则运算的使用实际: 极限都存在, 且分母不为0
3. **注意事项(不懂啊不懂)**
   1. 加减不可以用, 乘除法整体可以用
   2. 局部不可以用
   3. 函数内部不可以用

#### 5. 洛必达法则

#### 6. 泰勒公式

1. 泰勒公式注意事项

   ​	1.最后一项+ 最后一项的高阶无穷小

   ​		泰勒公式展开都是加到最后一项的高阶无穷小(注意高阶无穷小没有符号)

   2. 注意使用泰勒公式的时候, 高阶项和高阶无穷小必须写
   3. 基本上所有的题都可以使用泰勒公式, 不过有的时候使用泰勒公式比较复杂

2. **使用泰勒公式化简的原则**

   1. 分子分母同阶原则

   2. 系数不为0原则

   3. 我们展开泰勒公式的时候, 可以无穷无尽的去展开, 但是到哪一项就停止了呢

      就是根据分子和分母的幂次, 分母是6次幂, 那么我们就展开到6次幂就可以了

3. **三角函数的泰勒公式展开(重要)**

   1. $\sin x = x - \frac {x^3}{3!} + \frac {x^5}{5!} - \frac {x^7}{7!} + o*x^8 + o(x^8)  (这个是精确版本) \\ \;\;\;\;\;\;\;=x - \frac {x^3}{3!} + \frac {x^5}{5!} - \frac {x^7}{7!} +o(x^7)(这个是好记版本)$.

   2. $\cos x = 1 -\frac {x^2}{2!} + \frac {x^4}{4!} - \frac {x^6}{6!} + o * x^7 + o(x^7)(这个是精确版本) \\ \;\;\,\;\;\;\;\;=   1 -\frac {x^2}{2!} + \frac {x^4}{4!} - \frac {x^6}{6!} + o(x^6)(这个是好记版本)$ 

   3. 精确版本和好记版本都可以, 做简单题的时候, 两者没有什么区别

      不过当做难题的时候, 精确版本就能显式出力量了

   4. 三角函数记泰勒公式的方法

      ​	sin x是奇函数, 右侧也只能含有多项式的奇数次幂

      ​	cos x是偶函数, 泰勒公式展开应该是多项式的偶数次幂

      ​	正负号是正负正负交错出现

4. **指数函数的泰勒公式展开(重要)**

   $e^x = 1 + x + \frac {x^2}{2!} + \frac {x^3}{3!} + o(x^3)$

5. **对数函数的泰勒公式展开(重要)**

   ​	$\ln(1+x) = x-\frac {x^2}{2!} + \frac {x^3}{3!} + \cdots + \frac  {(-1)^n}{n+1} x^{n+1} + \cdots (-1< x <\leqslant1) $

6. **幂函数的泰勒公式展开(重要)**

   ​	$(1+x)^{\alpha} = 1 +\alpha x +\frac{\alpha} {(\alpha -1) {2!} } x^2 + o(x^2)$

7. 一些函数的泰勒公式展开

    	1. $\frac 1 {1-x} = 1 + x+ x^2 + \cdots + x^n + \cdots (注意|x| < 1) \\ \;\;\;\;\;\;= 1 + x+ x^2 + \cdots + x^n + o(	x^n)$
        	2. $\frac 1 {1+x} = 1 - x+ x^2 -x^3+ \cdots + (-1)^nx^n + \cdots (注意|x| < 1) \\ \;\;\;\;\;\;= 1 + x+ x^2 + \cdots + x^n + o(x^n)$



#### 7. 左右极限求函数极限

1. 函数极限的充分必要条件是左右极限存在且相等, 

   因此我们可以利用函数的左右极限来求函数极限

   $\lim\limits_{x\rightarrow x_{0}} f(x)= A \Longleftrightarrow \lim\limits_{x\rightarrow x_{0}^+} f(x) = \lim\limits_{x\rightarrow x_{0}^-} f(x)= A$

2. **一般使用左右极限的场景**

   1. 分段函数,在分段点左右的函数表达式不同
   2. $带有\frac 1x$这样的函数, 都要考虑左右极限
      1. $\frac 1x $
      2. $\arctan \frac 1x$
      3. $ \sin \frac 1x$
      4. $\cos \frac 1 x$
      5. $e^{\frac  1x}$



### 4. 函数极限反问题

1. 极限反问题的概念

   ​	以前我们是由表达式求极限, 现在是从极限的结果反求表达式的参数

   ​	这样的反过程就叫做函数极限的反问题

2. **第一个定理: 比值为A, 分母是无穷小, 则分子是无穷小(高阶无穷小/同阶无穷小)**

   ​	1.$如果\lim\limits_{x\rightarrow x_{0}} \frac {f(x)}{g(x)} = A且 \lim\limits_{x\rightarrow x_{0}} g(x) = 0 \\那么\lim\limits_{x\rightarrow x_{0}} f(x) = 0$

   2. 证明过程

      $\lim\limits_{x\rightarrow x_{0}} f(x) =\lim\limits_{x\rightarrow x_{0}} \frac {f(x)}{g(x)} * g(x) = 0$

2. **第二个定理: 比值为B(B不为0), 分子是无穷小, 则分母是无穷小**

   ​	$如果\lim\limits_{x\rightarrow x_{0}} \frac {f(x)}{g(x)} = B(B \neq  0), 且\lim\limits_{x\rightarrow x_{0}} f(x) = 0 \\那么\lim\limits_{x\rightarrow x_{0}} g(x) = 0$

## 4. 无穷大量和无穷小量

### 1. 无穷小量

1. **无穷小量的概念**

   ​	$如果\lim\limits_{x\rightarrow x_{0}}f(x) = 0, 那么就称f(x)是x\rightarrow x_{0}时的无穷小$	

   ​	如果函数的极限值是0, 那么就称这个表达式为无穷小量, 简称无穷小

   ​	只要函数的极限值是0, 那么这个函数就是无穷小

2. 无穷小量的注意事项

   ​	无穷小量不是一个数, 而是一个变化的过程(无穷小量是极限)

3. 常见的无穷小量举例
   1. $\lim\limits_{n\rightarrow x_{0}} \sin x^2= 0, 此时\sin x^2就是无穷小$
   2. $\lim\limits_{n\rightarrow x_{0}} \frac 1 {x^2+1}= 0, 此时\frac 1 {x^2+1}是无穷小$

4. **无穷小的性质**

   1. 有限个无穷小的和,差, 积仍然是无穷小, (隐含意思是无限个无穷小的和,差,积未必是无穷小)

   2. $无穷小* 有界= 无穷小$

   3. $如果f(x)的极限值为A, 那么f(x)=A+无穷小$

      $\lim\limits_{n\rightarrow x_{0}}f(x) = A \Longleftrightarrow \lim\limits_{n\rightarrow x_{0}} (f(x)-A)= 0 \\记作f(x)-A= \alpha(x)\\即f(x)= A+\alpha(x)$

   

### 2. 无穷大量

1. $如果\lim\limits_{n\rightarrow x_{0}}f(x) = \infty, 那么就称f(x)是x\rightarrow x_{0}时的无穷大$

2. **无穷大与无穷小之间是倒数关系**

   $如果\lim\limits_{n\rightarrow x_{0}}f(x) = \infty, 那么\lim\limits_{n\rightarrow x_{0}} \frac 1{f(x)} = 0$
   $如果\lim\limits_{n\rightarrow x_{0}}g(x) = 0, 那么\lim\limits_{n\rightarrow x_{0}} \frac 1{g(x)}= \infty (此时要求g(x) != 0)$

3. **无穷大和无界的关系**

   无穷大就是一直很大, 而无界有两种情况<1无穷大(一直很大), 2振荡>

   **因此无穷大一定是无界,但是无界不一定是无穷大**

   **$即无穷大  \Longrightarrow 无界, 但是无界  \nRightarrow 无穷大$**

### 3. 无穷小的阶的概念和定义

1. 无穷小的阶的理解及注意事项

   1. **考研的第一题一定是和无穷小的阶相关的**

   2. 无穷小的阶的前提条件是 $\lim\limits_{x\rightarrow x_{0}} \alpha(x) =0 且\lim\limits_{x\rightarrow x_{0}} \beta(x) =0$

   3. 注意无穷小的阶的前提条件是在自变量相同变化下的无穷小

   4. 无穷小的阶有点像比较的意思, 它实际上是刻画无穷小趋于0速度快慢的一个指标

      比如说飞机比火车快, 火车比汽车快, 汽车比自行车快

   5. **无穷小和泰勒公式的关系**

      无穷小更具有一般性,无穷小是泰勒公式的一种简化, 而不能说无穷小的本质是泰勒公式

   6. **无穷小和无穷大没有系数, 它们不是一个数, 而是一个动态的变化**

2. **高阶无穷小: 就是相比较而言, 分子趋于0的速度更快**

   1. $在\lim\limits_{x\rightarrow x_{0}} \alpha(x) =0 且\lim\limits_{x\rightarrow x_{0}} \beta(x) =0的前提条件下 \\如果\lim\limits_{x\rightarrow x_{0}} \frac {\alpha (x)} {\beta (x)} = 0, 那么称\alpha(x)是\beta(x)的高阶无穷小, 记为\alpha(x) = o(\beta (x))$

   2. 示例: $\lim\limits_{x\rightarrow x_{0}} \frac {x^3}{x}= \lim\limits_{x\rightarrow x_{0}} x^2 = 0 (注意x !=0)$
      因此我们就可以说, $分子x^3比分母x,在x\rightarrow0的时候的变化速度更快$

      比如$当x=0.01时, x^3= 0.01^3 < x = 0.01$

3. **低阶无穷小: 就是相比较而言, 分母趋于0的速度更快(分子趋于0的速度更慢)**

   1. $在\lim\limits_{x\rightarrow x_{0}} \alpha(x) =0 且\lim\limits_{x\rightarrow x_{0}} \beta(x) =0的前提条件下\\如果\lim\limits_{x**\rightarrow x_{0}} \frac {\alpha (x)} {\beta (x)} = \infty, 那么称\alpha(x)是\beta(x)的低阶无穷小, 记为\alpha(x) = O(\beta (x))$
      注意大O这个符号(O), 现在用的不多了, 虽然考研这个符号用的不多, 但是这个符号不会错

 4. **同阶无穷小: 就是相比较而言,分子和分母趋于0的速度差不多, 只差一个倍数, 差距没有特别大**

    1. $在\lim\limits_{x\rightarrow x_{0}} \alpha(x) =0 且\lim\limits_{x\rightarrow x_{0}} \beta(x) =0的前提条件下 \\如果\lim\limits_{x\rightarrow x_{0}} \frac {\alpha (x)} {\beta (x)} = c \;\;(c \neq 0), 那么称\alpha(x)是\beta(x)的同阶无穷小$

 5. **等价无穷小**(等价无穷小是我们求函数极限时最常用的)

    1. $在\lim\limits_{x\rightarrow x_{0}} \alpha(x) =0 且\lim\limits_{x\rightarrow x_{0}} \beta(x) =0的前提条件下\\如果\lim\limits_{x\rightarrow x_{0}} \frac {\alpha (x)} {\beta (x)} = 1, 那么称\alpha(x)是\beta(x)的等价无穷小, 记为\alpha(x) \thicksim \beta (x))$
    2. 我们可以将等价无穷小看作同阶无穷小的一个特例

6. **k阶无穷小**

   ​	1. $在\lim\limits_{x\rightarrow x_{0}} \alpha(x) =0 且\lim\limits_{x\rightarrow x_{0}} \beta(x) =0的前提条件下\\如果\lim\limits_{x\rightarrow x_{0}} \frac {\alpha (x)} {\beta^{k} (x)} = c (c \neq 0), 那么称\alpha(x)是\beta(x)的k阶无穷小, 记为\alpha(x) \thicksim \beta (x))$

### 4. 常见的等价无穷小(一般是$x\rightarrow 0$)

1. $当x\rightarrow 0时$(常用的, 需要背熟)

   1. $\sin x \thicksim \tan x \thicksim \arcsin x \thicksim \arctan x \thicksim x$
   2. $1-\cos x \thicksim \frac 1 2 x^2$
   3. $e^x - 1 ~ \thicksim x$
   4. $a^x - 1 = e^{x \ln a} - 1 \thicksim x\ln a$

   5. $\ln(1+x) \thicksim x$
   6. $(1+x)^\alpha -1 \thicksim a$

2. $当x\rightarrow 0时$高级一点的等价无穷小

   1. $x - \sin x \thicksim \frac 16x^3 $
   2. $\tan x -x \thicksim \frac 13x^3$
   3. $\tan x - \sin x = \frac 12 x^3$

3. $x - \ln(1+x) \thicksim \frac 12 x^3$

4. **等价无穷小的证明$\sin x  \thicksim x$**

   $\lim\limits_{x\rightarrow 0 } \frac {\sin x}{x} = 1 \Longrightarrow \sin x \Longrightarrow x$ 

5. **等价无穷小的证明**$e^x - 1 ~ \thicksim x$

   令$e^x -1 = t$

   $则\lim\limits_{x\rightarrow 0} \frac {e^x - 1}{x} = \lim\limits_{t\rightarrow 0} \frac{t} {\ln (1+t)} =\lim\limits_{t\rightarrow 0} \frac {1} { \frac 1t \ln(1+t)} = \lim\limits_{t\rightarrow 0} \frac {1}{ln(1+t)^{\frac 1t}} = \lim\limits_{t\rightarrow 0} \frac {1} {\ln e} = 1$

6. **等价无穷小的证明** $x - \ln(1+x) \thicksim \frac 12 x^3$: 这个使用泰勒公式来证明

   

### 5. 高阶无穷小的运算性质

1. $记住这一个: o(x^m)+o(x^n) = o(x^n)  (m > n)$ 

   $举例:当 x=0.01时, 0.01+0.01^2 \thicksim 0.01, 在趋于0的过程中, 幂次小的数反而大, 大就起支配作用, 就会在变化过程中起着支配作用$

2. $记住这一个: o(x^n) + o(x^n) = o(x^n)$

3. $k*o(x^n) = o(x^n)$

4. $o(x^m) * o(x^n) = o(x^{m+n})$

5. **高阶无穷小没有符号(即没有正负号), 不过我们一般写+** 

   ​	因此高阶无穷小减高阶无穷小还是等于高阶无穷小, 不是等于0

   ​	$即o(x^4) - o(x^4) = o(x^4)$

### 6. 等价无穷小替换原则

1. $如果\lim\limits_{x\rightarrow x_{0}} \alpha(x)= 0且\lim\limits_{x\rightarrow x_{0}} \beta(x), 且\alpha(x) \thicksim \beta(x) $
   $则\lim\limits_{x\rightarrow x_{0}} \frac {\alpha(x)}{\beta(x)} = \lim\limits_{x\rightarrow x_{0}} \frac {\alpha(x)}{\widetilde{\alpha(x)}} *\frac {\widetilde{\alpha(x)}}{\widetilde{\beta(x)}} *\frac {\widetilde{\alpha(x)}}{\beta(x)} =\lim\limits_{x\rightarrow x_{0}} 1 *\frac {\widetilde{\alpha(x)}}{\widetilde{\beta(x)}}  * 1 =  \lim\limits_{x\rightarrow x_{0}}\frac {\widetilde{\alpha(x)}}{\widetilde{\beta(x)}}  $
2. **注意事项(不懂啊不懂)**
   1. 加减不可以用, 乘除法整体可以用
   2. 局部不可以用
   3. 函数内部不可以用



# 四. 连续和间断

## 1. 连续性(点连续)

1. 点连续的概念

   ​	$点连续就是函数f(x)在x= x_{0}处连续, 连续就是指曲线是一笔划过来的, 没有分段\\不连续就是中间断了$

2. **使用极限来刻画点连续性**

   ​	我们画点连续性的时候很容易画, 基本上一幅图画就可以搞定	

   ​	但是在数学上我们需要使用数学语言来刻画点连续性, 使用的方案就是极限

   ​	$如果\lim\limits_{x\rightarrow x_{0}} = f(x_{0})称f(x)在x = x_{0}处连续$	

   ​	本质上来说, 函数连续就是极限等于函数在这一点的取值

3. 函数连续需要满足的三个条件

   1. 函数的极限存在

   2. 函数f(x)在x= x_{0}处有意义或者有定义

   3. 函数的极限等于函数在这一点的取值

      当这三个条件全部满足的时候, 我们才可以说, 函数f(x)在单点处连续

      本质上来说, 连续就是极限等于函数在这一点的取值

4. **函数点连续的充分必要条件**

   ​	$\lim\limits_{x\rightarrow x_{0}}=f(x_{0}) \Longleftrightarrow \lim\limits_{x\rightarrow x_{0}^-}= \lim\limits_{x\rightarrow x_{0}}=^+ = f(x_{0})$

5. 连续的使用场景: 分段函数在分段点的时候, 优先考虑用连续, 不过要注意分段函数在分段点的性质

6. **点连续的注意事项**
   1. 如果函数连续, 那么求极限的时候就直接代入了函数的取值了
   2. 初等函数在**定义域内**都连续(注意必须是在定义域内)
   3. 初等函数经过有限次的四则运算和有限次的复合运算之后仍然连续, 但是必须都在定义域内
   4. 我们目前介绍的是单点性连续(也叫做点连续), 而不是区间性连续, 区间性的连续我们还没有介绍

## 2. 连续函数

1. 连续函数的概念和定义

   ​	连续函数就是指区间上连续, 区间上连续是指区间上的每一点都连续

   ​	$f(x)在(a, b)上连续 \Longleftrightarrow 对于任意的x_{0} \in (a, b), f(x)在x_{0}上连续$

## 3. 间断点及其类型

1. **间断点相关概念**

   1. 间断点在函数中没有意义, 其实就只是一些特殊的点, 然后我们需要研究它
   2. 间断和连续是一个对立的概念, 不满足连续的时候就叫做间断

2. **第一类间断点**

   | 第一类间断点 | 函数的左极限和右极限都存在                                   |
   | ------------ | ------------------------------------------------------------ |
   | 可去间断点   | 函数的左右极限存在且相等, 称$x_{0}$为可去间断点, 一般是在$x_{0}$处屋顶一<br />因为这种间断点可以修正, 或者可以修复, 这种间断点就叫做可去间断点 |
   | 跳跃间断点   | 左右极限存在且不等, 称为跳跃间断点<br />因为这种间断点就是一个跳跃的状态 |

 3. **第二类间断点**

    | 第二类间断点 | 极限或右极限至少有一个不存在<br />函数极限不存在的情况:<1无穷. 2振荡> |
    | ------------ | ------------------------------------------------------------ |
    | 无穷间断点   | 左极限等于无穷或者右极限等于无穷, 称$x_{0}$为无穷间断点      |
    | 振荡间断点   | 振荡间断点不太好定义, 不过 $\sin \frac 1x 和 \cos \frac 1x是振荡间断点$ |

3. **间断点相关的出题: 寻找间断点并判断类型是我们考试的一个重要题型**
   1. 寻找间断点的方法: 找分母为0的点或者无定义的点
   2. 判断间断点的类型: 求左右极限, 根据左右极限的情况来判断间断点的类型

​			

## 4.有界闭区间

1. 有界闭区间[a, b]连续函数f(x)的性质  

   1. 闭区间的含义是包含两个端点
   2. 有界的含义是区间的两个端点a和b都不能是无穷
2. 有界闭区间的性质

| 最值定理<br />(最常用)     | 有界闭区间上的连续函数一定有最大值和最小值                   |
| :------------------------- | ------------------------------------------------------------ |
| 有界定理                   | 有界闭区间上的连续函数一定有界(函数值有上界或者下界)<br />$f(x_{0} ) = M, f(x_{1}) = m, 其中x_{0}和x_{1} \in [a, b]$ |
| **零点定理<br />(最常用)** | 如果有界闭区间[a, b]上的连续函数$f(x)满足f(a ) * f(b ) < 0$<br />$则一定存在一个f(\delta) = 0, 其中\delta \in (a, b)$ |
| 介质定理                   | 如果有界闭区间[a, b]上的连续函数f(x)有最大值M, 最小值m, 且$m \leqslant C \leqslant M$<br />那么则会有$f(n) = C, n \in [a, b]$ |

**