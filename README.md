# 理论计算机科学导引

这个仓库用于整理《理论计算机科学导引》的课程笔记。

## 笔记列表

- [Week 1 整理笔记](./理论计算机科学导引_Week1_整理笔记.md)
- [Week 2 整理笔记](./理论计算机科学导引_Week2_整理笔记.md)
- [Week 3 整理笔记](./理论计算机科学导引_Week3_整理笔记.md)

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
