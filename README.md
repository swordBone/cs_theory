# 理论计算机科学导引

这个仓库用于整理《理论计算机科学导引》的课程笔记。

## 小测复习

- [Week 1-5 小测复习汇总](./理论计算机科学导引_Week1-5_小测复习汇总.md)：公式速查、核心证明、构造例题、易错点和 12 道自测题及参考答案。

## 笔记列表

- [Week 1 整理笔记](./理论计算机科学导引_Week1_整理笔记.md)
- [Week 2 整理笔记](./理论计算机科学导引_Week2_整理笔记.md)
- [Week 3 整理笔记](./理论计算机科学导引_Week3_整理笔记.md)
- [Week 4 整理笔记](./理论计算机科学导引_Week4_整理笔记.md)
- [Week 5 整理笔记](./理论计算机科学导引_Week5_整理笔记.md)

## L5 专题补充

根据新增的 `L5_0_1793243778225.pdf` 整理。原理按 Week 4、Week 5 通读，下面三篇用于练习转换和非正则性证明；[专题目录](./notes/l5-automata/README.md)提供材料页码与阅读路线。

- [ε 闭包与子集构造练习](./notes/l5-automata/01-subset-construction.md)：初始闭包、字符后的闭包、空集陷阱与完整转移表。
- [正则表达式与状态消除例题](./notes/l5-automata/02-regular-expressions-and-elimination.md)：`(01∪0)*` 的 ε-NFA，以及 1 的个数模 3 余 1 的消除过程。
- [泵引理与非正则性证明](./notes/l5-automata/03-pumping-lemma.md)：量词、鸽巢证明、等量 0/1 与平方长度语言、带答案自测。

## 作业解答

- [作业 2 解答](./作业2_解答.md)：正则语言的补集、两个四状态 NFA 构造、含空转移的 NFA 转 DFA、正则表达式及重复串语言的抽引引理证明。

## 习题解答 / Exercise Solutions

- [在线阅读最新版 PDF / Read the latest PDF](https://swordbone.github.io/cs_theory/solutions.pdf)
- [第 2、3、5 章选题解答（中英双语 LaTeX）](./习题解答_2_3_5章.tex)
- [自动编译状态与历史 / Build status and history](https://github.com/swordBone/cs_theory/actions/workflows/latex-pdf.yml)

涵盖 2.4、2.5(1)、2.14、3.9、3.14、5.1、5.2、5.3、5.4、5.9，包含完整中文及英文证明。
其中 5.4 包含对原题无限制输出长度表述的反例，以及修正版的计数证明。

在 Overleaf 中将 **Compiler** 设为 **XeLaTeX** 后编译；不要使用默认的 pdfLaTeX。
文件前半部分为中文解答，后半部分为英文解答，可从目录跳转。GitHub 文件页展示 `.tex` 源代码；上方固定链接提供编译后的 PDF。

The LaTeX document contains complete Chinese and English solutions to all ten exercises.
Compile with **XeLaTeX**; in Overleaf, select it explicitly in the project's **Compiler** settings.

### 自动编译与发布

推送到 `main` 且修改了解答 `.tex`、工作流或 PDF 跳转页时，GitHub Actions 会使用 XeLaTeX 自动编译，并在成功后更新 GitHub Pages 上的 PDF。也可在 Actions 的 **Build and publish PDF** 中点击 **Run workflow** 手动运行。

Pull request 只编译检查，不发布。编译失败时不会覆盖上一次成功发布的 PDF；可在运行记录的 `latex-build-log` 附件中查看日志。
每次成功编译还会提供 `exercise-solutions-pdf` 附件，保留 30 天；固定阅读链接始终指向最近一次成功发布的版本，不受附件保留期影响。

GitHub Actions compiles relevant changes on `main` with XeLaTeX and publishes the PDF only after a successful build. Pull requests are checked without deployment. The permanent PDF link serves the latest successful publication; downloadable build artifacts are retained for 30 days.

## 内容索引

| 周次 | 主要内容 |
| --- | --- |
| Week 1 | 问题与函数、编码、可数性与不可计算性 |
| Week 2 | 布尔电路与 NAND、加法、LOOKUP、分块共享与 $`O(m2^n/n)`$ 上界 |
| Week 3 | SIZE、程序编码与计数下界、规模层级定理、通用求值器 EVAL |
| Week 4 | 变长输入与语言、DFA/NFA、正则语言、并集与连接封闭性、子集构造 |
| Week 5 | DFA/NFA 等价、Kleene 星、正则表达式、Thompson 构造、状态消除法与路径递推 |

## 数学公式显示

请在文件页选择 **Preview** 阅读；**Code** 和 **Raw** 显示的是源代码。行内公式使用 GitHub 支持的美元符号加反引号写法，独立公式使用 `math` 围栏，参见 [GitHub 数学公式文档](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)。

第四周已将 GitHub 页面实际拒绝的 `\operatorname` 写法改为兼容的 `\mathrm`。后续检查既要验证 TeX 语法，也要检查 GitHub 的实际预览；仅在本地能渲染不代表平台一定接受全部命令。程序、真值表和伪代码仍保留代码块，不属于未渲染公式。
