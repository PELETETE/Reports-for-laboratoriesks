# MathMode.tex - Basic Math Mode Introduction {#sec:mathmode}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \begin{document}
    A sentence with inline mathematics: $y = mx + c$.

    A second sentence with inline mathematics: $5^{2}=3^{2}+4^{2}$.
    %A second paragraph containing display math.
    \[
     y = mx + c
    \]
    %See how the paragraph continues after the display.
    \end{document}

## Generated figure {#generated-figure .unnumbered}

Basic inline and display math mode examples.

## Screenshot {#screenshot .unnumbered}

::: center
![image](MathMode.png){width="80%"}
:::

------------------------------------------------------------------------

# MathModeSuperscripts.tex - Superscripts and Subscripts {#sec:superscripts}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \begin{document}
    Superscripts $a^{b}$ and subscripts $a_{b}$.
    \end{document}

## Generated figure {#generated-figure-1 .unnumbered}

Demonstration of superscript and subscript notation.

## Screenshot {#screenshot-1 .unnumbered}

::: center
![image](MathModeSuperscripts.png){width="60%"}
:::

------------------------------------------------------------------------

# MathModeCommands.tex - Math Commands {#sec:commands}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \begin{document}
    Some mathematics: $y = 2 \sin \theta^{2}$.
    \end{document}

## Generated figure {#generated-figure-2 .unnumbered}

Using mathematical functions like `\sin` and Greek letters.

## Screenshot {#screenshot-2 .unnumbered}

::: center
![image](MathModeCommands.png){width="60%"}
:::

------------------------------------------------------------------------

# DisplayMathematics.tex - Display Mathematics {#sec:display}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \begin{document}
    A paragraph about a larger equation
    \[
    \int_{-\infty}^{+\infty} e^{-x^2} \, dx
    \]
    \end{document}

## Generated figure {#generated-figure-3 .unnumbered}

Display math with integral and Gaussian function.

## Screenshot {#screenshot-3 .unnumbered}

::: center
![image](DisplayMathematics.png){width="70%"}
:::

------------------------------------------------------------------------

# DisplayMathematicsEquation.tex - Numbered Equations {#sec:equation}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \begin{document}
    A paragraph about a larger equation
    \begin{equation}
    \int_{-\infty}^{+\infty} e^{-x^2} \, dx
    \end{equation}
    \end{document}

## Generated figure {#generated-figure-4 .unnumbered}

Numbered equation using `equation` environment.

## Screenshot {#screenshot-4 .unnumbered}

::: center
![image](DisplayMathematicsEquation.png){width="70%"}
:::

------------------------------------------------------------------------

# DisplayMathematicsDiff.tex - Custom Differential {#sec:diff}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \newcommand{\diff}{\mathop{}\!d} % For italic
    % \newcommand{\diff}{\mathop{}\!\mathrm{d}} % For upright
    \begin{document}
    A paragraph about a larger equation
    \[
    \int_{-\infty}^{+\infty} e^{-x^2} \diff x
    \]
    \end{document}

## Generated figure {#generated-figure-5 .unnumbered}

Custom differential command for better spacing.

## Screenshot {#screenshot-5 .unnumbered}

::: center
![image](DisplayMathematicsDiff.png){width="70%"}
:::

------------------------------------------------------------------------

# TheAmsmathPackage.tex - AMS Math Package Introduction {#sec:amsmath}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{amsmath}
    \begin{document}
    Solve the following recurrence for $ n,k\geq 0 $:
    \begin{align*}
      Q_{n,0} &= 1 \quad Q_{0,k} = [k=0]; \\
      Q_{n,k} &= Q_{n-1,k}+Q_{n-1,k-1}+\binom{n}{k},\quad\text{for $n$, $k>0$.}
    \end{align*}
    \end{document}

## Generated figure {#generated-figure-6 .unnumbered}

AMS align environment for multi-line equations.

## Screenshot {#screenshot-6 .unnumbered}

::: center
![image](TheAmsmathPackage.png){width="80%"}
:::

------------------------------------------------------------------------

# TheAmsmathPackageMatrices.tex - AMS Matrices {#sec:matrices}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{amsmath}
    \begin{document}
    AMS matrices.
    \[
    \begin{matrix}
    a & b & c \\
    d & e & f
    \end{matrix}
    \quad
    \begin{pmatrix}
    a & b & c \\
    d & e & f
    \end{pmatrix}
    \quad
    \begin{bmatrix}
    a & b & c \\
    d & e & f
    \end{bmatrix}
    \]
    \end{document}

## Generated figure {#generated-figure-7 .unnumbered}

Different matrix environments from amsmath.

## Screenshot {#screenshot-7 .unnumbered}

::: center
![image](TheAmsmathPackageMatrices.png){width="80%"}
:::

------------------------------------------------------------------------

# ColumnsinMathAlignments.tex - Column Alignments {#sec:columns}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{amsmath}
    \begin{document}
    Aligned equations
    \begin{align*}
    a &= b+1 & c &= d+2 & e &= f+3 \\
    r &= s^{2} & t &=u^{3} & v &= w^{4}
    \end{align*}
    \end{document}

## Generated figure {#generated-figure-8 .unnumbered}

Multiple columns in align environment.

## Screenshot {#screenshot-8 .unnumbered}

::: center
![image](ColumnsinMathAlignments.png){width="80%"}
:::

------------------------------------------------------------------------

# DisplayingEnvironmentAmsmathAlignments.tex - Aligned Subenvironment {#sec:aligned}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{amsmath}
    \begin{document}
    \begin{itemize}
    \item
    $\begin{aligned}[t]
    a&=b\\
    c&=d
    \end{aligned}$
    \item
    $\begin{aligned}
    a&=b\\
    c&=d
    \end{aligned}$
    \end{itemize}
    \end{document}

## Generated figure {#generated-figure-9 .unnumbered}

Aligned subenvironment with vertical positioning.

## Screenshot {#screenshot-9 .unnumbered}

::: center
![image](DisplayingEnvironmentAmsmathAlignments.png){width="60%"}
:::

------------------------------------------------------------------------

# FurtherAmsmathAlignments.tex - Gather and Multline {#sec:further}

    \documentclass[a4paper]{article}
    \usepackage[T1]{fontenc}
    \usepackage{amsmath}
    \begin{document}
    Gather
    \begin{gather}
      P(x)=ax^{5}+bx^{4}+cx^{3}+dx^{2}+ex +f\\
      x^2+x=10
    \end{gather}
    Multline
    \begin{multline*}
       (a+b+c+d)x^{5}+(b+c+d+e)x^{4} \\
        +(c+d+e+f)x^{3}+(d+e+f+a)x^{2}+(e+f+a+b)x\\
        + (f+a+b+c)
    \end{multline*}
    \end{document}

## Generated figure {#generated-figure-10 .unnumbered}

Gather and multline environments for multi-line equations.

## Screenshot {#screenshot-10 .unnumbered}

::: center
![image](FurtherAmsmathAlignments.png){width="80%"}
:::

------------------------------------------------------------------------

# BoldMath.tex - Bold Mathematics {#sec:boldmath}

    \documentclass[a4paper]{article}
    \usepackage[T1]{fontenc}

    \begin{document}

    $(x+y)(x-y)=x^{2}-y^{2}$

    {\boldmath $(x+y)(x-y)=x^{2}-y^{2}$ $\pi r^2$}
    $(x+\mathbf{y})(x-\mathbf{y})=x^{2}-{\mathbf{y}}^{2}$
    $\mathbf{\pi} r^2$ % bad use of \mathbf
    \end{document}

## Generated figure {#generated-figure-11 .unnumbered}

Bold math using `\boldsymbol` and `\mathbf`.

## Screenshot {#screenshot-11 .unnumbered}

::: center
![image](BoldMath.png){width="80%"}
:::

------------------------------------------------------------------------

# FontsinMathModeBoldface.tex - Boldface in Math {#sec:boldface}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \begin{document}
    The matrix $\mathbf{M}$.
    \end{document}

## Generated figure {#generated-figure-12 .unnumbered}

Bold math symbols.

## Screenshot {#screenshot-12 .unnumbered}

::: center
![image](FontsinMathModeBoldface.png){width="50%"}
:::

------------------------------------------------------------------------

# FontsinMathModeSpecifics.tex - Math Font Specifics {#sec:fonts}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{amsmath}
    \begin{document}
    $\text{bad use } size \neq \mathit{size} \neq \mathrm{size} $
    \textit{$\text{bad use } size \neq \mathit{size} \neq \mathrm{size} $}
    \end{document}

## Generated figure {#generated-figure-13 .unnumbered}

Different math font styles.

## Screenshot {#screenshot-13 .unnumbered}

::: center
![image](FontsinMathModeSpecifics.png){width="80%"}
:::

------------------------------------------------------------------------

# Mathtools.tex - Mathtools Package {#sec:mathtools}

    \documentclass[a4paper]{article}
    \usepackage[T1]{fontenc}
    \usepackage{mathtools}
    \begin{document}
    \[
    \begin{pmatrix*}[r]
    10&11\\
    1&2\\
    5&-4
    -5&-6
    \end{pmatrix*}
    \]
    \end{document}

## Generated figure {#generated-figure-14 .unnumbered}

Mathtools package with starred matrix for alignment.

## Screenshot {#screenshot-14 .unnumbered}

::: center
![image](Mathtools.png){width="60%"}
:::

------------------------------------------------------------------------

# BoldMathCommendBM.tex - pmatrix\* Environment {#sec:bm}

    \documentclass[a4paper]{article}
    \usepackage[T1]{fontenc}
    \usepackage{mathtools}
    \begin{document}
    \[
    \begin{pmatrix*}[r]
    10&11\\
    1&2\\
    -5&-6
    \end{pmatrix*}
    \]
    \end{document}

## Generated figure {#generated-figure-15 .unnumbered}

Matrix with right-aligned negative numbers.

## Screenshot {#screenshot-15 .unnumbered}

::: center
![image](BoldMathCommendBM.png){width="60%"}
:::

------------------------------------------------------------------------

# LualatexMathMode.tex - Unicode Math with LuaLaTeX {#sec:lualatex}

    \documentclass[a4paper]{article}
    \usepackage{unicode-math}
    \setmainfont{TeX Gyre Pagella}
    \setmathfont{TeX Gyre Pagella Math}
    \begin{document}
    One two three
    \[
    \log \alpha + \log \beta = \log(\alpha\beta)
    \]

    Unicode Math Alphanumerics
    \[A + \symfrak{A}+\symbf{A}+ \symcal{A} + \symscr{A}+\symbb{A}\]
    \end{document}

## Generated figure {#generated-figure-16 .unnumbered}

LuaLaTeX with unicode-math for modern font handling.

## Screenshot {#screenshot-16 .unnumbered}

::: center
![image](LualatexMathMode.png){width="80%"}
:::

------------------------------------------------------------------------

# Lab03MathMode.tex - Comprehensive Lab Examples {#sec:lab03}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \begin{document}
    %%  3-1) Math Mode
     A sentence with inline mathematics: $y = mx + c$.
     A second sentence with inline mathematics: $5^{2}=3^{2}+4^{2}$.


     A second paragraph containing display math.
     \[
      y = mx + c
     \]
     See how the paragraph continues after the display.
     \end{document}

    \textasciitilde
     %% 3-2) Examples where simple super- and subscripts are entered without braces
     \usepackage[T1]{fontenc}
     \begin{document}
     Superscripts $a^{b}$ and subscripts $a_{b}$.
     \end{document}


    \textasciitilde
    documentclass[a4paper]{article}
    \usepackage[T1]{fontenc}
    \usepackage{mathtools}
    \begin{document}
    \[
    \begin{pmatrix*}[r]
    10&11\\
    1&2\\
    -5&-6
    \end{pmatrix*}
    \]
    \end{document}


    \end{document}

## Generated figure {#generated-figure-17 .unnumbered}

Multiple examples combined from laboratory exercises.

## Screenshot {#screenshot-17 .unnumbered}

::: center
![image](Lab03MathMode.png){width="80%"}
:::

------------------------------------------------------------------------

# Conclusion: Methodology for Mathematical Typesetting {#conclusion-methodology-for-mathematical-typesetting .unnumbered}

After comprehensive analysis of mathematical mode examples, here is the
structured methodology for effective mathematical typesetting in LaTeX:

## 1. Essential math mode structures {#essential-math-mode-structures .unnumbered}

    % Inline math: $...$ or \(...\)
    $E = mc^2$

    % Display math unnumbered: \[...\]
    \[
    \int_a^b f(x)\,dx
    \]

    % Display math numbered: \begin{equation}...\end{equation}
    \begin{equation}
    \sum_{i=1}^n i = \frac{n(n+1)}{2}
    \end{equation}

    % Multi-line equations: \begin{align}...\end{align}
    \begin{align}
    x &= y + z \\
    u &= v + w
    \end{align}

## 2. Math mode environments comparison {#math-mode-environments-comparison .unnumbered}

  **Environment**   **Package**   **Purpose**
  ----------------- ------------- ---------------------------------------------
  `equation`        amsmath       Numbered single equation
  `align`           amsmath       Multi-line alignment with multiple columns
  `gather`          amsmath       Multi-line equations without alignment
  `multline`        amsmath       Single equation split over multiple lines
  `matrix`          amsmath       Unbracketed matrix
  `pmatrix`         amsmath       Matrix with parentheses
  `bmatrix`         amsmath       Matrix with square brackets
  `pmatrix*`        mathtools     Matrix with column alignment options
  `aligned`         amsmath       Subenvironment for blocks within other math

## 5. Essential practices {#essential-practices .unnumbered}

::: framed
**Best practices for mathematical typesetting:**

1\. **Always use math mode for mathematics**: Never use regular text for
mathematical symbols

2\. **Load amsmath**: It's essential for professional math typesetting

3\. **Use appropriate brackets**: For matrices, choose the right bracket
style

4\. **Be careful with bold**: Use `\mathbf` for variables, `\boldsymbol`
for symbols

5\. **Differentiate d and e**: Consider upright d for differential,
italic e for Euler's number

6\. **Align at equals signs**: Use `&` in align environments

7\. **Label important equations**: Use `\label` and `\ref` for
cross-referencing

**Final** : Mastering mathematical typesetting is essential for
scientific writing. Start with simple inline math, progress to displayed
equations, then advance to multi-line alignments and matrices. Always
use the appropriate packages (amsmath, mathtools) and choose the
compilation engine that best suits your needs. Well-formatted
mathematics enhances readability and professionalism of academic
documents.
:::
