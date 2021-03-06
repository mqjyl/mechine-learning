# 概率论

概率论（随机数学）：数学的一个分支，研究如何定量描述随机现象及其规律。

数理统计：以数据为唯一研究对象， 包括数据的收集、整理、分析和建模。从而对随机现象的某些规律进行预测或决策。

**最重要的两个词：随机 和 数据**

## ✏ **随机事件**

自然界与社会生活中的两类现象**：**确

* 确定性现象：在一定条件下必然发生的现象。
* 随机现象：在一定条件下具有多种可能结果， 且 试验时无法预知出现哪个结果的现象。

对随机现象的观察、记录、实验统称为 `随机试验`，它具有以下特性： 

* 可以在相同条件下重复进行； 
* 事先知道所有可能出现的结果； 
* 进行试验前并不知道哪个试验结果会发生。

`样本空间`：随机试验的所有可能结果构成的 集合称为样本空间，记为 $$S=\{e\}$$ ， S中的元素 e 称为样本点。

`随机事件`：样本空间S的子集A称为随机事件A，简称事件A。当且仅当A中的某个样本点发生称 事件A发生。 事件A的表示可用集合，也可用语言来表示。

如果把S看作事件，则每次试验S总是发生，所以S称 为必然事件；如果事件只含有一个样本点，称其为基本事件； 如果事件是空集，里面不包含任何样本点，记为 $$\phi$$ ， 则每次试验 $$\phi$$ 都不发生，称 $$\phi$$ 为不可能事件。

## ✏ 频率 和 概率

### 🖋 频率

频率是0～1之间的一个实数，在大 量重复试验的基础上给出了随机事 件发生可能性的估计，频率定义：

$$
f_n(A) = \frac{n_A}{n}
$$

其中 $$n_A$$ 是 $$A$$ 发生的次数（频数），n 是总试验次数，称 $$f_n(A)$$ 为 $$A$$ 在这 n 次试验中发生频率。

#### 频率的性质：

* $$0 \le f_n(A)\le1$$ 
* $$f_n(S) = 1$$ 
* 若 $$A_1,A_2,\ldots,A_k$$ 两两互不相容，则 $$f_n(\bigcup_{i = 1}^k A_i) = \sum_{i = 1}^k f_n(A_i)$$ 

频率的重要性质： $$f_n(A)$$ 随 n 的增大渐趋稳定，稳定值为 p。

### 🖋 概率

概率的统计性定义： 当试验的次数增加时，随机事件 $$A$$ 发生的频率的稳定值 p 称为概率.记为 $$P(A)=p$$ 。

概率的公理化定义：设随机试验对应的样本空间为 $$S$$ ，对每个事件 A，定义 $$P(A)$$ 满足：

1. 非负性： $$P(A)\ge 0$$ ；
2. 规范性： $$P(S)=1$$ ；
3. 可列可加性：$$A_1,A_2,\ldots$$ 两两互斥，即 $$A_i A_j = \phi, i \neq j$$ ，则 $$P(\bigcup_{i = 1}^{\infty} A_i) = \sum_{i = 1}^{\infty} P(A_i)$$ 。

称 $$P(A)$$ 为事件 A 的概率。

#### 重要性质：

1、若 $$A\subset B$$ ，则有 $$P(B - A) = P(B) - P(A)$$ ，一般情况下， $$P(B - A) = P(B) - P(AB)$$ 

2、概率加法公式： $$P(A \cup B) = P(A) + P(B) - P(AB)$$ ，推广：

$$P(A \cup B \cup C) = P(A) + P(B) + P(C) - P(AB) - P(AC) - P(BC) + P(ABC)$$ 

$$P(\bigcup_{i = 1}^n A_i) = \sum_{i = 1}^nP(A_i) - \sum_{1\le i < j \le n}P(A_i A_j) + \sum_{1\le i < j < k \le n}P(A_i A_j A_k) + \cdots + (-1)^{n - 1}P(A_1 A_2\cdots A_n)$$ 

