---
author:
- PELE TETE
date: December 2025
title: "LABORATORY08: Report and Presentation of work on TikZ"
---

# 801TikZ - Basic LaTeX Document {#sec:801}

    \documentclass[a4paper,12pt]{article}
    \usepackage[T1]{fontenc}
    \begin{document}
    \section{This is a simple introduction to TikZ}
    There is a variety of different toolsets for creating graphical objects in a TeX doc
    ument. Themostwellknownandprobablymostwidelyusedofthesetoolsetsis
    TikZ, which is a recursive acronym for “TikZ ist kein Zeichenprogramm” (German
    for TikZ is not a drawing programme). Fromthenameofthetoolsetyoucansee
    that generating a figure in TikZ will not work through drawing the figure like you
    might befamiliar with doing in Paint or similar drawing programmes. To create a
    figure using TikZ we will need to code it by using specific TeX commands. We will
    take a look at the basics of TikZ here.
    Three useful references and sources of inspiration for creating TikZ figure are:

    • TheWikibooksentryonTikZ:https://en.wikibooks.org/wiki/LaTeX/PGF/TikZ.
    • TheCTANentryonTikZwiththeofficialhandbookandotherdocumentation:
    https://www.ctan.org/pkg/pgf.

    • TheTeXampleTikZdatabasefullofexamplesandinspiration: https://texa
    mple.net/tikz/.

    My work is extremely based on the first link. In the following lines, 
    we will see how we can code by using TikZ.
    \end{document}

## Generated figure (simulation) {#generated-figure-simulation .unnumbered}

Standard text document without TikZ graphics.

## Imported image {#imported-image .unnumbered}

::: center
![image](801TikZ.png){width="80%"}
:::

------------------------------------------------------------------------

# 802TikZ.tex - Introduction to key concepts {#sec:802}

    \documentclass[a4paper,12pt]{article}
    \usepackage[T1]{fontenc}
    \begin{document}
    In this section, we will talking about five(05) Importants keys.
    To succeed to work from TikZ
    First to remember to start coding by \usepackage{tikz}
    second use \begin{figure} this helps us make the reference.
    third use \begin{tikzpicture} in other to manage the graphic.
    fouth never forget to close by \end{tikzpicture}
    at the and we have the rule the use of semicolon(';').
    \end{document}

## Generated figure (simulation) {#generated-figure-simulation-1 .unnumbered}

Explanatory text about TikZ.

## Screenshot {#screenshot .unnumbered}

::: center
![image](802TikZ.png){width="80%"}
:::

------------------------------------------------------------------------

# 803TikZDrawinglines - Drawing simple lines {#sec:803}

    \documentclass{article}
    \usepackage{tikz}
    \begin{document}
    \begin{tikzpicture}
    \draw (-1,0) -- (3,10pt) -- (35:3);
    \end{tikzpicture}
    \end{document}

## Generated figure {#generated-figure .unnumbered}

::: center
:::

## Screenshot {#screenshot-1 .unnumbered}

::: center
![image](803TikZDrawinglines.png){width="60%"}
:::

------------------------------------------------------------------------

# 804TikZDrawinglines - Line styles {#sec:804}

    \documentclass{article}
    \usepackage{tikz}
    \begin{document}
    \begin{tikzpicture}
    \draw[->] (-1,0) -| (3,10pt);
    \draw[red] (3,10pt) -- (35:3);
    \end{tikzpicture}
    \end{document}

## Generated figure {#generated-figure-1 .unnumbered}

::: center
:::

## Screenshot {#screenshot-2 .unnumbered}

::: center
![image](804TikZDrawinglines.png){width="60%"}
:::

------------------------------------------------------------------------

# 805TikZDrawinglines - Curves with controls {#sec:805}

    \documentclass{article}
    \usepackage{tikz}
    \begin{document}
    \begin{tikzpicture}
    \draw (-1,0) to (5,1);
    \draw[green] (-1,0) to[out=90,in=135] (5,1);
    \draw[cyan] (-1,0) .. controls (0,-2) .. (5,1);
    \end{tikzpicture}
    \end{document}

## Generated figure {#generated-figure-2 .unnumbered}

::: center
:::

## Screenshot {#screenshot-3 .unnumbered}

::: center
![image](805TikZDrawinglines.png){width="60%"}
:::

------------------------------------------------------------------------

# 806TikZDrawinglines - Advanced curves {#sec:806}

    \documentclass{article}
    \usepackage{tikz}
    \begin{document}
    \begin{tikzpicture}
    \draw[dotted,gray] (-1,0) -- (5,1);
    \draw (-1,0) .. controls (0,-2) and (4,2) .. (5,1);
    \end{tikzpicture}
    \end{document}

## Generated figure {#generated-figure-3 .unnumbered}

::: center
:::

## Screenshot {#screenshot-4 .unnumbered}

::: center
![image](806TikZDrawinglines.png){width="60%"}
:::

------------------------------------------------------------------------

# 810TikZNodes - Introduction to nodes {#sec:810}

    \documentclass{article}
    \usepackage{tikz}
    \begin{document}
    \begin{tikzpicture}[scale=4]
    \draw (0,0) node {hello} -- (1,1) node {world};
    \end{tikzpicture}
    \end{document}

## Generated figure {#generated-figure-4 .unnumbered}

::: center
:::

## Screenshot {#screenshot-5 .unnumbered}

::: center
![image](810TikZNodes.png){width="60%"}
:::

------------------------------------------------------------------------

# 811TikZNodes - Node positioning {#sec:811}

    \documentclass{article}
    \usepackage{tikz}
    \begin{document}
    \begin{tikzpicture}[scale=3]
    \draw (0,0) -- (1,1) node[midway]{A} node[pos=0.75,above]{B} node[right]{C};
    \draw (0,0) -- (1,1) node[left]{D};
    \end{tikzpicture}
    \end{document}

## Generated figure {#generated-figure-5 .unnumbered}

::: center
:::

## Screenshot {#screenshot-6 .unnumbered}

::: center
![image](811TikZNodes.png){width="60%"}
:::

------------------------------------------------------------------------

# 812TikZNodes - Nodes with 'to' command {#sec:812}

    \documentclass{article}
    \usepackage{tikz}
    \begin{document}
    \begin{tikzpicture}[scale=3]
    \draw (0,0) to node[midway]{A} node[pos=0.75, above]{B} (1,1) node[right]{C};
    \end{tikzpicture}
    \end{document}

## Generated figure {#generated-figure-6 .unnumbered}

::: center
:::

## Screenshot {#screenshot-7 .unnumbered}

::: center
![image](812TikZNodes.png){width="60%"}
:::

------------------------------------------------------------------------

# 813TikZNodes.tex - Mathematical forms {#sec:813}

    \documentclass{article}
    \usepackage{tikz}
    \begin{document}
    \begin{tikzpicture}[scale=3]
    \draw (0,0) node[circle, draw]{$\sum_{i=1}^{n}n^2$} -- (1,1)
    node[rectangle,draw]{$\frac{1}{\sqrt{2}}$};
    \end{tikzpicture}
    \end{document}

## Generated figure {#generated-figure-7 .unnumbered}

::: center
:::

## Screenshot {#screenshot-8 .unnumbered}

::: center
![image](813TikZNodes.png){width="60%"}
:::

------------------------------------------------------------------------

# 814TikZNodes - Named nodes {#sec:814}

    \documentclass{article}
    \usepackage{tikz}
    \begin{document}
    \begin{tikzpicture}[scale=3]
    \node[circle,draw] (label1) at (0,0) {$\sum_{i=1}^{n}n^2$};
    \node[rectangle,draw] (label2) at (1,1) {$\frac{1}{\sqrt{2}}$};
    \draw (label1) -- (label2);
    \end{tikzpicture}
    \end{document}

## Generated figure {#generated-figure-8 .unnumbered}

::: center
:::

## Screenshot {#screenshot-9 .unnumbered}

::: center
![image](814TikZNodes.png){width="60%"}
:::

------------------------------------------------------------------------

# 815TikZNodesGenerateGraph - Complex graph {#sec:815}

    \documentclass{article}
    \usepackage{tikz}
    \begin{document}
    \begin{tikzpicture}[scale=2]
    \node[circle, draw] at (0,0) (a) {A};
    \node[rectangle, fill] at (3,0) (b) {};
    \node at (3,0.4) (blabel) {B};
    \node[rectangle,rounded corners, draw] at (5,2) (c) {C};

    \draw[->, green] (a) -- (b) node[midway, below,black]{2};
    \draw[<->, blue] (a) to[out=45, in=135] (b);
    \draw[->,red] (b)--(c);
    \draw[yellow,dotted,very thick] (b) |- (c);
    \draw[<-,cyan] (b) -| (c);
    \draw[thick,black] (a).. controls (1,5) .. (c) 
        node[midway,above]{$\frac{1}{2}$};
    \end{tikzpicture}
    \end{document}

## Generated figure {#generated-figure-9 .unnumbered}

::: center
:::

## Screenshot {#screenshot-10 .unnumbered}

::: center
![image](815TikZNodesGenerateGraph.png){width="70%"}
:::

------------------------------------------------------------------------

# 820Plottingcurves - Simple curve plotting {#sec:820}

    \documentclass{article}
    \usepackage{tikz}
    \begin{document}
    \begin{tikzpicture}
    \draw [domain=-2:2] plot (\x, {pow(\x,2)});
    \end{tikzpicture}
    \end{document}

## Generated figure {#generated-figure-10 .unnumbered}

::: center
:::

## Screenshot {#screenshot-11 .unnumbered}

::: center
![image](820Plottingcurves.png){width="60%"}
:::

------------------------------------------------------------------------

# 821APlottingcurves - Cosine with axes {#sec:821A}

    \documentclass{article}
    \usepackage{tikz}
    \begin{document}
    \begin{tikzpicture}[scale=1.5]
    \draw[gray, ->] (-2,0) -- (2,0) node[right]{$x$} node[pos=0.53, below]{$O$};
    \draw[gray, ->] (0,-1) -- (0,1) node[above]{$y$};
    \draw[fill,gray] (0,0) circle [radius=1pt];
    \draw[blue, thick] [domain=-2:2, samples=50] 
        plot (\x,{cos(pi*\x r)})
        node[right]{$y = \cos(x)$};
    \end{tikzpicture}
    \end{document}

## Generated figure {#generated-figure-11 .unnumbered}

::: center
:::

## Screenshot {#screenshot-12 .unnumbered}

::: center
![image](821APlottingcurves.png){width="70%"}
:::

------------------------------------------------------------------------

# 821BPlottingcurves - Parabola with axes {#sec:821B}

    \documentclass{article}
    \usepackage{tikz}
    \begin{document}
    \begin{tikzpicture}
    \draw[gray, ->] (-3,0) -- (3,0) node[right]{$x$} node[pos=0.53, below]{$O$};
    \draw[gray, ->] (0,-2) -- (0,2) node[above]{$y$};
    \draw[fill,gray] (0,0) circle [radius=1pt];
    \draw [domain=-2:2] plot (\x, {pow(\x,2)}) node[right] {$y = x^2$};
    \end{tikzpicture}
    \end{document}

## Generated figure {#generated-figure-12 .unnumbered}

::: center
:::

## Screenshot {#screenshot-13 .unnumbered}

::: center
![image](821BPlottingcurves.png){width="70%"}
:::

------------------------------------------------------------------------

# 830TikZWorkingWithLoops - Simple loops {#sec:830}

    \documentclass{article}
    \usepackage{tikz}
    \begin{document}
    \begin{tikzpicture}[scale=0.75]
    \foreach \x in {0,1,2,3}
    \draw[red,thick] (0,\x) circle [radius=\x+1];
    \end{tikzpicture}
    \end{document}

## Generated figure {#generated-figure-13 .unnumbered}

::: center
:::

## Screenshot {#screenshot-14 .unnumbered}

::: center
![image](830TikZWorkingWithLoops.png){width="60%"}
:::

------------------------------------------------------------------------

# 831TikZWorkingWithLoopsSierpiński - Sierpiński triangle {#sec:831}

    \documentclass[border=1cm]{standalone}
    \usepackage{tikz}
    \usetikzlibrary{math}

    \newcommand\Triangle[2]{
      \draw #1 coordinate(a)-- ++(0:#2) coordinate(b);
      \draw (a)-- ++(60:#2) coordinate(c);
      \fill (a)-- (b)-- (c)-- cycle;
    }

    \begin{document}
    \begin{tikzpicture}
      \tikzmath{
        function sierpinski(\x, \y, \s, \d) {
          if (\d == 0) then {
            { \Triangle{(\x,\y)}{\s}; };
          } else {
            \u1 = 0.25*\s;
            \u2 = \u1*sqrt(3);
            \u3 = 0.5*\s;
            sierpinski(\x,\y,\u3,\d-1);
            sierpinski(\x+\u3,\y,\u3,\d-1);
            sierpinski(\x+\u1,\y+\u2,\u3,\d-1);
          };
        };
     \S = 4; 
        for \d in {0,...,5}{
          % To situate all plots nicely under and next to each other, define the coords
          % of the lower left corners preemptively
          \x = (\S+1)*mod(\d,2);
          \y = int(\d/2) * (\S+1);
          sierpinski(\x,-\y,\S,\d);
          };
      }
    \end{tikzpicture}
    \end{document}

## Generated figure {#generated-figure-14 .unnumbered}

::: center
:::

## Screenshot {#screenshot-15 .unnumbered}

::: center
![image](831TikZWorkingWithLoopsSierpiński.png){width="80%"}
:::

------------------------------------------------------------------------

# 840EXERCICE1 - Exercise: Pentagon {#sec:840}

    \documentclass{article}
    \usepackage{tikz}
    \begin{document}
    \begin{tikzpicture}
    \foreach \a/\i in {0/1,72/2,144/3,216/4,288/5}
        \node[circle,draw] (v\i) at (\a:2) {$v_{\i}$};
    \draw (v1)--(v2)--(v3)--(v4)--(v5)--cycle;
    \draw[red] (v1)--(v3)--(v5)--(v2)--(v4)--cycle;
    \end{tikzpicture}
    \end{document}

## Generated figure {#generated-figure-15 .unnumbered}

::: center
:::

## Screenshot {#screenshot-16 .unnumbered}

::: center
![image](840Exercice1.png){width="60%"}
:::

------------------------------------------------------------------------

# 841EXERCICE - Exponential and logarithmic functions {#sec:841}

    \documentclass[border=1cm]{standalone}
    \usepackage{tikz}
    \usepackage{amsmath}
    \begin{document}
    \begin{tikzpicture}[>=stealth, scale=1.2]
        \draw[very thin, gray!30] (-2,-2) grid (4,4);
        \draw[->, thick] (-2.5,0) -- (4.5,0) node[right] {$x$};
        \draw[->, thick] (0,-2.5) -- (0,4.5) node[above] {$y$};
        \node[below left] at (0,0) {$O$};
        \draw[blue, thick, domain=-2.2:1.4, samples=50] 
            plot (\x, {exp(\x)}) node[right] {$y=e^x$};
        \draw[red, thick, domain=0.12:4.2, samples=50] 
            plot (\x, {ln(\x)}) node[above right] {$y=\ln(x)$};
        \filldraw[blue] (0,1) circle (2pt);
        \node[left, blue] at (0,1) {$A(0,1)$};
        \filldraw[red] (1,0) circle (2pt);
        \node[below right, red] at (1,0) {$B(1,0)$};
    \end{tikzpicture}
    \end{document}

## Generated figure {#generated-figure-16 .unnumbered}

::: center
:::

## Screenshot {#screenshot-17 .unnumbered}

::: center
![image](841Exercice.png){width="70%"}
:::

------------------------------------------------------------------------

# 842EXERCICE3 - Fractal tree {#sec:842}

    \documentclass[border=1cm]{standalone}
    \usepackage{tikz}
    \usetikzlibrary{math}
    \begin{document}
    \begin{tikzpicture}[x=1cm, y=1cm]
      \tikzmath{
        function drawtree(\x, \y, \angle, \size, \depth) {
          if (\depth > 0) then {
            \nextx = \x + \size * cos(\angle);
            \nexty = \y + \size * sin(\angle);
            {
              \draw[line width=\size*2, color=green!\depth!brown] 
                (\x, \y) -- (\nextx, \nexty);
            };
            \newsize = \size * 0.75;
            \newdepth = \depth - 1;
            drawtree(\nextx, \nexty, \angle + 25, \newsize, \newdepth);
            drawtree(\nextx, \nexty, \angle - 35, \newsize, \newdepth);
          };
        };
        drawtree(0, 0, 90, 1.5, 9);
      }
    \end{tikzpicture}
    \end{document}

## Generated figure {#generated-figure-17 .unnumbered}

::: center
:::

## Screenshot {#screenshot-18 .unnumbered}

::: center
![image](842Exercice3.png){width="70%"}
:::

------------------------------------------------------------------------

# Conclusion: Methodology for creating successful TikZ documents {#conclusion-methodology-for-creating-successful-tikz-documents .unnumbered}

After exhaustive study of TikZ examples, here is the structured
methodology for creating successful TikZ documents:

## 1. Essential basic structure {#essential-basic-structure .unnumbered}

    \documentclass{article}  % or standalone for figures only
    \usepackage{tikz}        % REQUIRED first
    \usepackage{amsmath}     % For mathematical formulas
    % Other packages as needed
    \begin{document}
    \begin{tikzpicture}[options]
      % Your TikZ code here
    \end{tikzpicture}
    \end{document}

## 2. Recommended progressive approach {#recommended-progressive-approach .unnumbered}

**Step 1: Planning**

- Define dimensions (min/max coordinates)

- Identify graphical elements (lines, shapes, text)

- Choose appropriate scale

**Step 2: Build in layers**

1.  Reference grid (`draw[gray, thin] (0,-8) grid (5,5);`)

2.  Axes and reference marks

3.  Main elements

4.  Details and annotations

5.  Legends and text

**Step 3: Optimize**

- Use custom styles: `\tikzset{monstyle/.style={red, thick}}`

- Define reusable nodes

- Organize with relative coordinates

## 3. Essential best practices {#essential-best-practices .unnumbered}

  **Practice**             **Example**
  ------------------------ --------------------------------------------
  Comment code             `% X-axis`
  Name nodes               `(A) at (0,0)`
  Use loops                `\foreach` for repetitions
  Separate style/content   Styles in preamble, drawing in tikzpicture
  Test frequently          Compile often to detect errors

## 4. Synthetic conclusion {#synthetic-conclusion .unnumbered}

::: framed
**To create successful TikZ documents:**

1\. **Structure**: Preamble → Environment → Commands → Closure

2\. **Iterate**: Simple → Complex, Grid → Axes → Shapes → Details

3\. **Optimize**: Styles, Loops, Named nodes

4\. **Verify**: Semicolons, Names, Scale

5\. **Document**: Comments, Separate files, Notes
:::

**Final reminder**: TikZ is a powerful tool requiring practice. Always
start with simple examples, gradually increase complexity, and don't
hesitate to break down complex figures into several independent
`tikzpicture` environments.
