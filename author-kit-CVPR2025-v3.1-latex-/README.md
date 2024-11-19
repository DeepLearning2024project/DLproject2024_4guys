# CVPR/ICCV/3DV Official LaTeX template 

**Note:** the Microsoft Word version of the template is in the branch [`main-msword`](https://github.com/cvpr-org/author-kit/tree/main-msword).

### History (in reverse chronological order)

- added styles for `subsubsection` and fixed the wrong PDF bookmarks by [Di Fang](https://github.com/fang-d)
- modernized for CVPR 2025 by [Christian Richardt](https://richardt.name/)
- fixed page centering for CVPR 2025 by [Stefan Roth](mailto:stefan.roth@NOSPAMtu-darmstadt.de)
- inline enumerations and `cvprblue` links for CVPR 2025 by [Ioannis Gkioulekas
](https://www.cs.cmu.edu/~igkioule/)
- added automated LaTeX build testing for CVPR 2025 by [Ahan Shabanov](https://ahanio.github.io)
- references in `cvprblue` for CVPR 2024 by [Klaus Greff](https://github.com/Qwlouse) 
- added natbib for CVPR 2024 by [Christian Richardt](https://richardt.name/)
- replaced buggy (review-mode) line numbering for 3DV 2024 by [Adín Ramírez Rivera
](https://openreview.net/profile?id=~Ad%C3%ADn_Ram%C3%ADrez_Rivera1)
- logic for inline supplementary for 3DV 2024 by [Andrea Tagliasacchi](https://taiya.github.io) 
- modernized for CVPR 2022 by [Stefan Roth](mailto:stefan.roth@NOSPAMtu-darmstadt.de)
- created cvpr.sty file to unify review/rebuttal/final versions by [Ming-Ming Cheng](https://github.com/MCG-NKU/CVPR_Template)
- developed CVPR 2005 template  by [Paolo Ienne](mailto:Paolo.Ienne@di.epfl.ch) and [Andrew Fitzgibbon](mailto:awf@acm.org)

------------------------------------------------------------------------------
以上是模板中自带的内容。考虑到大家对latex的熟悉程度，以下将对此模板的文件结构做一定的说明

- .github: 【folder】【不重要】一个隐藏的文件夹，GitHub 用它来存放与 GitHub Actions 相关的配置文件。（GitHub Actions 是 GitHub 的自动化功能，在仓库中执行自动化任务）
  - workflows: 【folder】【不重要】
- sec: 【folder】section的缩写，**存放论文中各个章节的内容**
- `cvpr.sty`: 【file】【不重要】LaTeX 样式文件，包含 CVPR的论文格式规范。**定义了文档布局、字体、标题等**
- `ieeenat_fullname.bst`: 【不重要】BibTeX 样式文件，用于**格式化参考文献列表**
- `main.bib`: **_存储文献引用信息。在 LaTeX 文档中引用的文献都要在这个文件中列出_**
- `main.tex`: **主文件**
- `preamble.tex`: 【不重要】包含了 LaTeX 文档的导言区（preamble），即 \documentclass 和 \begin{document} 之间的部分，包括宏包的引入和文档的设置
- `rebuttal.tex`: 【不重要】回应审稿人意见的反驳信