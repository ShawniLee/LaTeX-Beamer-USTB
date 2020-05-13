# Beamer-Style-of-USTB
北京科技大学LaTeX-beamer幻灯片模板

两个模板对在LaTeX中常用的格式，包括itemize, enumerate, description, 图片，表格，代码，伪代码等等，都给出了示例。

两个模板都支持以gb7714-2015标准所规定的格式排版参考文献。

<br/>

## LaTeX beamer style for University of Science and Technology Beijing

[LaTeX beamer style for USTB](./beamer_nankai)
1. These files are initially based on [南开大学模板](https://github.com/zshicode/LaTeX-Beamer-Nankai),
2. This is an unofficial LaTeX beamer style for USTB, the style file is `nkcolor.sty` and the example file is `slides.tex`.
3. Link to Thesis Templates：[南开大学本科生毕业论文LaTeX模板](https://github.com/kongxiao0532/NKU_Bachelor_Thesis_Template)，[南开大学硕博毕业论文LaTeX模板](https://github.com/NewFuture/NKThesis)

To compile the slides, use:
```
xelatex slides
biber slides
xelatex slides
xelatex slides
```
and you can get the PDF.
<br/>

## Report Template

[Report Template](./report_template)

To compile the report, use:
```
xelatex report
biber report
xelatex report
xelatex report
```
and you can get the PDF.

## Others

As you have noticed, other LaTeX styles or even Markdown styles are also included in the folder [single_file_model](./single_file_model), such as `typora_monokai.css`, `document_model.tex`, `warsaw_beamer_model.tex`. They are single, simple and basic. The `deepblue.sty` is a LaTeX beamer style based on `nkcolor.sty`, but I don't use an image as background or logo in this style, and the theme color is deep blue.

[A LaTeX theme of Python](./python_theme_beamer) is also available. The `pycolor.sty`, and the example of using this style is given by `pyeg.tex`. This file use the `pythonhighlight.sty`, the package is loaded by the following line:

```tex
\usepackage{pythonhighlight}
```

It is then possible to include a Python snippet directly in the code using:

```tex
\begin{python}
def f(x):
    return x
\end{python}
```

It is also possible to include inline Python code in LaTeX with ``\pyth``:

```tex
The special method \pyth{__init__}... 
```

Last but not least, you can load an external Python file with:

```tex
\inputpython{python_file.py}{23}{50}
```

to display the contents of the file ``python_file`` from line 23 to line 50.

What's more, the `mcode.sty` gives a implementation to highlight MATLAB .m-code in LaTeX.
