GMU Proposal 干净模板

这是从当前文件夹提取的可复用模板，不含原作者的研究正文、图片、个人信息和文献库。
gmuETD.sty 原样保留；main.tex 保留原模板作者署名和声明。
样式来自本地文件（包含 2023 年修订记录），未核验最新 GMU 提交要求。
Proposal 封面由本地定制封面改为占位符，不表示学校统一要求的开题格式。

使用方法
1. 将对应 ZIP 作为新项目上传到 Overleaf。
2. 主文件选 main.tex，编译器选 pdfLaTeX。
3. 在 metadata.tex 修改姓名、题目、院系、导师、委员等信息。
4. 在 chapters/ 中填写自己的正文；增加章节时，在 main.tex 加相应的 \include。
5. references.bib 留空。添加自己的文献和 \cite{文献键} 后，
   取消 main.tex 中 \bibliographystyle 和 \bibliography 两行前面的 %。
6. 按需启用 main.tex 中注释的附录、图目录、表目录（如有）。
7. 保留一个空白 Overleaf 项目作为母版，每次新写作复制项目。
   下载项目源码 ZIP 可备份并再次导入；下载 PDF 只得到排版结果。

文件说明
main.tex             主文件与章节顺序
metadata.tex         个人信息（英文占位符）
gmuETD.sty           原始 GMU 排版样式
chapters/            正文章节占位符
references.bib       自己的参考文献
appendix.tex         可选附录
proposal-cover.tex   可编辑的开题封面

本模板的正文为英文；中文说明在本文件中，不参与 LaTeX 编译。
本地编译：latexmk -pdf main.tex
