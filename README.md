# Math Reasoning Post-Training

数学推理模型后训练实验与外推评测展示。

[SFT-Full](#sft-full) · [SFT-LoRA](#sft-lora) · [GRPO](#grpo) · [2026 高考全国一卷](#2026-高考全国一卷)

---

## SFT-Full

> 结果待补充。

## SFT-LoRA

> 结果待补充。

## GRPO

> 结果待补充。

## 2026 高考全国一卷

这里将 2026 年全国一卷数学客观题作为基模后训练的 benchmark 外推测试。除了常见 benchmark，我们也引入更新、与训练数据时间分布不同的题目，观察模型面对新题时的数学推理与作答表现。

本卷共 14 道客观题，满分 73 分。成绩同时报告真实高考分数和严格全对题数。

### 成绩排行

| 排名 | 考生 | 成绩 | 百分比 | 严格全对 | 状态 |
| ---: | --- | ---: | ---: | ---: | --- |
| 1 | Qwen2.5-3B | **41 / 73** | **56.16%** | **8 / 14** | 已完成 |
| — | GPT | — | — | — | 待测 |
| — | Claude | — | — | — | 待测 |
| — | DeepSeek | — | — | — | 待测 |

> 当前排行仅包含已有真实评测结果的模型；待测模型不参与名次计算。

### 评分口径

- 单选题每题 5 分，答错或未提取到答案得 0 分。
- 多选题含错误选项得 0 分；正确答案为两个选项时，只选一个正确项得 3 分；正确答案为三个选项时，只选一个正确项得 2 分、只选两个正确项得 4 分。
- 填空题每题 5 分；多空答案按顺序严格全对计分。
- “严格全对”只统计获得该题满分的题目。

### 考生答卷

**GPT（待测）** · **Claude（待测）** · **DeepSeek（待测）** · **Qwen2.5-3B（当前展示）**

#### Qwen2.5-3B

| 项目 | 成绩 | 百分比 | 严格全对 |
| --- | ---: | ---: | ---: |
| 总成绩 | **41 / 73** | **56.16%** | **8 / 14** |
| 选择题 | 36 / 58 | 62.07% | 7 / 11 |
| 填空题 | 5 / 15 | 33.33% | 1 / 3 |

<details>
<summary><strong>第 1 题 · 单选题 · 5 / 5 分 ✓</strong></summary>

样本数据 $6,8,4,5,12$ 的中位数为（$\quad$）

- (A) $5$
- (B) $6$
- (C) $8$
- (D) $9$

**模型答案：** B  
**正确答案：** B

</details>

<details>
<summary><strong>第 2 题 · 单选题 · 5 / 5 分 ✓</strong></summary>

已知平面向量 $\boldsymbol{a},\boldsymbol{b}$ 不共线，且 $2\boldsymbol{a}+y\boldsymbol{b}=x\boldsymbol{a}-3\boldsymbol{b}$，则（$\quad$）

- (A) $x=2,\ y=-3$
- (B) $x=-2,\ y=3$
- (C) $x=2,\ y=3$
- (D) $x=-2,\ y=-3$

**模型答案：** A  
**正确答案：** A

</details>

<details>
<summary><strong>第 3 题 · 单选题 · 5 / 5 分 ✓</strong></summary>

已知集合 $A=\left\{\sin\frac{7\pi}{6},\cos\frac{5\pi}{3},\tan\frac{5\pi}{4}\right\}$，$B=\left\{-\frac{\sqrt{3}}{2},-\frac{1}{2},1\right\}$，则 $A\cap B=$（$\quad$）

- (A) $\left\{-\frac{\sqrt{3}}{2},-\frac{1}{2}\right\}$
- (B) $\left\{-\frac{\sqrt{3}}{2},1\right\}$
- (C) $\left\{-\frac{1}{2},1\right\}$
- (D) $\left\{-\frac{\sqrt{3}}{2},-\frac{1}{2},1\right\}$

**模型答案：** C
**正确答案：** C

</details>

<details>
<summary><strong>第 4 题 · 单选题 · 5 / 5 分 ✓</strong></summary>

曲线 $y=5x+8\ln x$ 在点 $(1,5)$ 处的切线方程为（$\quad$）

- (A) $y=3x+2$
- (B) $y=5x$
- (C) $y=8x-3$
- (D) $y=13x-8$

**模型答案：** D  
**正确答案：** D

</details>

<details>
<summary><strong>第 5 题 · 单选题 · 5 / 5 分 ✓</strong></summary>

已知抛物线 $C_1:y^2=2p_1x\ (p_1>0)$ 和 $C_2:x^2=2p_2y\ (p_2>0)$ 均经过点 $(4,8)$，则 $C_1$ 的焦点与 $C_2$ 的焦点之间的距离为（$\quad$）

- (A) $12$
- (B) $4\sqrt{5}$
- (C) $6$
- (D) $\frac{\sqrt{65}}{2}$

**模型答案：** D  
**正确答案：** D

</details>

<details>
<summary><strong>第 6 题 · 单选题 · 0 / 5 分 ✗</strong></summary>

已知函数 $f(x)=\frac{x+2}{e^x+a}$ 的最大值为 $1$，则 $a=$（$\quad$）

- (A) $\frac{1}{2}$
- (B) $1$
- (C) $\frac{3}{2}$
- (D) $2$

**模型答案：** 模型循环输出
**正确答案：** B

</details>

<details>
<summary><strong>第 7 题 · 单选题 · 5 / 5 分 ✓</strong></summary>

一百零八塔位于宁夏回族自治区青铜峡市，以其独特的建筑格局和深远的历史文化闻名遐迩。该塔群共有 $108$ 座塔，依山势自上而下排成 $12$ 行，将第 $i$ 行中塔的座数记为 $a_i\ (i=1,2,\cdots,12)$，其中 $a_1=1$，$a_7=a_4=3$，$a_{11}=a_{12}=5$，且 $a_1,a_2,\cdots,a_{12}$ 是一个首项为 $7$、公差为 $2$ 的等差数列。将 $a_1,a_2,\cdots,a_{12}$ 分为 $6$ 组，每组 $2$ 个数，使得每组的 $2$ 个数之和可构成一个项数为 $6$ 且公差为 $d\ (d>0)$ 的等差数列，则 $d=$（$\quad$）

- (A) $2$
- (B) $4$
- (C) $6$
- (D) $8$

**模型答案：** B  
**正确答案：** B

</details>

<details>
<summary><strong>第 8 题 · 单选题 · 0 / 5 分 ✗</strong></summary>

设 $U=\{(x_1,x_2,x_3)\mid x_i\in\{-2,-1,1,2\},\ i=1,2,3\}$ 为由空间中 $64$ 个点构成的集合，点 $P(1,1,1)$，记样本空间 $\Omega=C_U(P)$。从 $\Omega$ 中随机取一个点。对 $\Omega$ 中的每个点 $A(x_1,x_2,x_3)$，令 $X(A)=x_1+x_2+x_3$，则 $X$ 的数学期望为（$\quad$）

- (A) $-\frac{1}{21}$
- (B) $-\frac{1}{63}$
- (C) $0$
- (D) $\frac{1}{7}$

**模型答案：** C  
**正确答案：** A

</details>

<details>
<summary><strong>第 9 题 · 多选题 · 6 / 6 分 ✓</strong></summary>

设 $z=3+2i$，则（$\quad$）

- (A) $\overline{z}=3-2i$
- (B) $|z|=5$
- (C) $z^2=5+12i$
- (D) $\frac{z+3}{z-i}\in\mathbb{R}$

**模型答案：** ACD  
**正确答案：** ACD

</details>

<details>
<summary><strong>第 10 题 · 多选题 · 0 / 6 分 ✗</strong></summary>

在空间中，$A,B$ 为两个定点，动点 $C$ 到直线 $AB$ 的距离为 $2$，动点 $D$ 到直线 $AB$ 的距离为 $1$。若二面角 $C-AB-D$ 为 $60^\circ$，则（$\quad$）

- (A) $\angle CAD\geqslant60^\circ$
- (B) $CD\geqslant\sqrt{3}$
- (C) 当 $AB\perp CD$ 时，$CD\perp$ 平面 $ABD$
- (D) 当 $AB\perp$ 平面 $ACD$ 时，$AC\perp AD$

**模型答案：** AB  
**正确答案：** BC

</details>

<details>
<summary><strong>第 11 题 · 多选题 · 0 / 6 分 ✗</strong></summary>

已知圆 $C_1:(x+1)^2+y^2=1$，圆 $C_2:(x-1)^2+y^2=1$，圆 $C_3:x^2+(y-\sqrt{3})^2=1$，直线 $l:y=kx+b$ 与 $C_1,C_2,C_3$ 均有两个交点。记 $C_1,C_2,C_3$ 截得的弦长分别为 $s_1,s_2,s_3$，则（$\quad$）

- (A) $k$ 可以取任意实数
- (B) 满足 $s_1=s_2=s_3$ 的直线 $l$ 共有 $3$ 条
- (C) 满足 $s_1+s_2+s_3=3$ 的直线 $l$ 多于 $3$ 条
- (D) 当 $b=0$ 时，$s_1+s_2+s_3$ 的最大值为 $\frac{2\sqrt{21}}{3}$

**模型答案：** ABD  
**正确答案：** BCD

</details>

<details>
<summary><strong>第 12 题 · 填空题 · 5 / 5 分 ✓</strong></summary>

双曲线 $5x^2-6y^2=1$ 的离心率为______。

**模型答案：** $\sqrt{\frac{11}{6}}$  
**正确答案：** $\sqrt{\frac{11}{6}}$

</details>

<details>
<summary><strong>第 13 题 · 填空题 · 0 / 5 分 ✗</strong></summary>

已知 $f(x)=2\sin(ax+\theta)\ (a\in\mathbb{Z},\ 0\leqslant\theta<2\pi)$ 是偶函数；$f(x)$ 在区间 $(0,\frac{\pi}{2})$ 单调递增，则 $\theta=$______，$f(\frac{2\pi}{3})=$______。

**模型答案：** $\pi;\sqrt{3}$  
**正确答案：** $\frac{3\pi}{2};1$

</details>

<details>
<summary><strong>第 14 题 · 填空题 · 0 / 5 分 ✗</strong></summary>

设实数 $q$ 满足：存在数列 $\{a_n\}$，使得对于任意 $n\in\mathbb{N}^*$，均有 $a_1+a_2+\cdots+a_n=n^2+n$，且 $\{a_n\}$ 中有某连续 $9$ 项 $a_i,a_{i+1},\cdots,a_{i+8}$ 是公比为 $q$ 的等比数列，则 $q$ 的最大值为______。

**模型答案：** $\frac{9}{8}$  
**正确答案：** $4$

</details>

---

评测数据来自项目本地 `gaokao_2026_math_objective` benchmark；本展示不包含训练代码、评测代码或原始日志。
