# 複数の PDF を1つのファイルに結合する

以下の内容の対象 PDF の名前を適宜変更し (英数字じゃないとダメかも)、LaTeX のファイル形式 `.tex` で保存してから `pdflatex (filename).tex` を実行する。
```
\documentclass[flegn]{article}
\usepackage{pdfpages}
\begin{document}
\includepdf[pages=-]{1.pdf}
\includepdf[pages=-]{2.pdf}
\includepdf[pages=-]{3.pdf}
\includepdf[pages=-]{4.pdf}
\includepdf[pages=-]{5.pdf}
\includepdf[pages=-]{6.pdf}
\includepdf[pages=-]{7.pdf}
\includepdf[pages=-]{8.pdf}
\includepdf[pages=-]{9.pdf}
\end{document}
```