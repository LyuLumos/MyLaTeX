# MyLaTeX

- Only support English.
- Base on [CTAN - mcmthesis](https://www.ctan.org/pkg/mcmthesis)
- [GPL-v3.0](LICENSE)

## Use

add [`head.tex`](head.tex) at the begin of your `.tex` file.

### Content
`Content` will be automatically completed according to `section` & `subsection`.

Of course you can use `subsubsection` if you like. :)

```latex
\tableofcontents
```
![](imgs/2021-08-17-18-13-32.png)


### Section

Three commands are supported: `section`, `subsection` and `subsubsection`.

```latex
\section{VC R-CNN}
\subsection{Intro}
\subsubsection{Example}
```

![](imgs/2021-08-17-17-43-51.png)

### Figure

```latex
\begin{figure}[h]
\small
\centering
\includegraphics[width=5cm]{commense} % figures/commense.png
\caption{Motivation of VC R-CNN}
\label{fig:moti1} % You can use `\eqref{fig:moti1}` to cite this figure.
\end{figure}
```

It is easy to use this block. However, I recommand you to create a new folder named `figures`. And you can only use `commense` instead of `figures/commense.png`

![](imgs/2021-08-17-17-50-47.png)


### Equation

You can use both `equation` or `align` as you like.



```latex
\begin{equation}
    \mathbb{E}_{\boldsymbol{z}}\left[\operatorname{Softmax}\left(f_{y}(\boldsymbol{x}, \boldsymbol{z})\right)\right] \stackrel{\mathrm{NWGM}}{\approx} \operatorname{Softmax}\left(\mathbb{E}_{\boldsymbol{z}}\left[f_{y}(\boldsymbol{x}, \boldsymbol{z})\right]\right)
    \label{equ: nwgm} % You can use `\eqref{equ: nwgm}` to cite this equation.
\end{equation}
```

![](imgs/2021-08-17-18-09-32.png)

### Hyperlink
```latex
\href{https://github.com/Wangt-CN/VC-R-CNN}{https://github.com/Wangt-CN/VC-R-CNN (Pytorch)}
```

![](imgs/2021-08-17-18-21-30.png)

### Code 

Only six languages supported in default config:  `C, C++, Python, Java, Matlab, Mathematica`

```latex
\lstinputlisting[language=Python]{./code/base.py} 
```
![](imgs/2021-08-17-18-01-30.png)

### Reference

I recommand to create a `.bib` file. You can only add this at the end of the `.tex` file.

```latex
\bibliographystyle{plain}
\bibliography{ref} % .bib file name
```

![](imgs/2021-08-17-18-18-01.png)

Use `\cite{}` to cite it.

![](imgs/2021-08-17-18-18-42.png)

