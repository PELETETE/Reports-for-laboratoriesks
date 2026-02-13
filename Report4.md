# l4-1a.tex - Basic Image Inclusion {#sec:l4-1a}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{graphicx}
    \begin{document}
    This picture.
    \begin{center}
        \includegraphics[height=6cm]{faucon.jpg}
    \end{center}
    is an imported PDF
    \end{document}

## Generated figure {#generated-figure .unnumbered}

Basic image inclusion with fixed height.

## Screenshot {#screenshot .unnumbered}

::: center
![image](l4-1a.png){width="80%"}
:::

## Analysis {#analysis .unnumbered}

This document demonstrates:

- Loading the `graphicx` package for image support

- Using `\includegraphics[height=6cm]{faucon.jpg}` to set fixed height

- Centering the image with `center` environment

------------------------------------------------------------------------

# l4-1b.tex - Relative Dimensions {#sec:l4-1b}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{graphicx}
    \begin{document}
    \begin{center}
        \includegraphics[height = 5cm\textheight]{faucon.jpg}
    \end{center}
    Here you can see faucon in the first image and corbeau in the second
    \begin{center}
        \includegraphics[width = 6cm\textwidth]{corbeau.jpg}
    \end{center}
    \end{document}

## Generated figure {#generated-figure-1 .unnumbered}

Images sized relative to text height and text width.

## Screenshot {#screenshot-1 .unnumbered}

::: center
![image](l4-1b.png){width="80%"}
:::

## Analysis {#analysis-1 .unnumbered}

This document demonstrates:

- Relative sizing: `height = 5cm\textheight`

- Relative sizing: `width = 6cm\textwidth`

- Two images (faucon and corbeau) in the same document

------------------------------------------------------------------------

# l4-1c.tex - Clipping and Trimming {#sec:l4-1c}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{graphicx}
    \begin{document}
    \begin{center}
        \includegraphics[clip, trim = 0 0 60 70]{faucon.png}
    \end{center}
    \end{document}

## Generated figure {#generated-figure-2 .unnumbered}

Image with clipping and trimming.

## Screenshot {#screenshot-2 .unnumbered}

::: center
![image](l4-1c.png){width="80%"}
:::

## Analysis {#analysis-2 .unnumbered}

This document demonstrates:

- `clip` option to enable trimming

- `trim = left bottom right top` to crop image edges

- Removing 60pt from right and 70pt from bottom

------------------------------------------------------------------------

# l4-2a.tex - Figure Environment with Captions {#sec:l4-2a}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{graphicx}
    \begin{document}
    Test location.
    \begin{figure}[ht]
      \centering
      \includegraphics[width=0.8\textwidth]{faucon.jpg}
      \caption{faucon en haut}
      \includegraphics[height=5cm]{corbeau.jpg}
      \caption{corbeau en bas}
    \end{figure}
    \end{document}

## Generated figure {#generated-figure-3 .unnumbered}

Float environment with multiple images and captions.

## Screenshot {#screenshot-3 .unnumbered}

::: center
![image](l4-2a.png){width="80%"}
:::

## Analysis {#analysis-3 .unnumbered}

This document demonstrates:

- `figure` float environment with placement specifier `[ht]`

- `\centering` for horizontal alignment

- `\caption` for figure descriptions

- Multiple images in a single float

------------------------------------------------------------------------

# l4-2b.tex - Float Placement Options {#sec:l4-2b}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{graphicx}
    \begin{document}
    Some text before the figure.

    \begin{figure}[h]
    \centering
    \includegraphics[width=0.5\textwidth]{corbeau.jpg}
    \caption{corbeau}
    \end{figure}

    More text after the figure.
    \end{document}

## Generated figure {#generated-figure-4 .unnumbered}

Float placement with \[h\] option.

## Screenshot {#screenshot-4 .unnumbered}

::: center
![image](l4-2b.png){width="80%"}
:::

## Analysis {#analysis-4 .unnumbered}

This document demonstrates:

- `[h]` placement specifier for \"here\"

- Width specified as 0.5\\textwidth

- Basic figure float structure

------------------------------------------------------------------------

# Thelabelandrefmechanism.tex - Labels and References {#sec:labelref}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \begin{document}
    \section{Introduction}
    Some exciting text with a reference~\ref{sec:next}.
    \section{Next thing}
    \label{sec:next}
    More text here.
    \end{document}

## Generated figure {#generated-figure-5 .unnumbered}

Cross-referencing mechanism.

## Screenshot {#screenshot-5 .unnumbered}

::: center
![image](Thelabelandrefmechanism.png){width="80%"}
:::

## Analysis {#analysis-5 .unnumbered}

This document demonstrates:

- `\label{sec:next}` to mark a section

- `\ref{sec:next}` to reference it

- Automatic numbering and cross-referencing

- Requires two compilation passes

------------------------------------------------------------------------

# Makingcross-referencesintolinks.tex - References with Figures {#sec:hyperref}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{graphicx}
    \begin{document}
    \section{Introduction}
    Some exciting text with a reference to Section~\ref{sec:next}.

    \section{corbeau et faucon}
    \label{sec:next}
    \begin{figure}[ht]
      \centering
      \includegraphics[width=0.8\textwidth]{faucon.jpg}
      \caption{faucon en haut}
      \includegraphics[height=5cm]{corbeau.jpg}
      \caption{corbeau en bas}
    \end{figure}
    More text here.
    \end{document}

## Generated figure {#generated-figure-6 .unnumbered}

Combined cross-references and figures.

## Screenshot {#screenshot-6 .unnumbered}

::: center
![image](Makingcross-referencesintolinks.png){width="80%"}
:::

## Analysis {#analysis-6 .unnumbered}

This document demonstrates:

- Integration of cross-references with figures

- Section label and reference

- Multiple images with captions in float

- Complete document structure

------------------------------------------------------------------------

# Naminggraphicsfiles.tex - File Naming Issues {#sec:naming}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{graphicx}
    \begin{document}
    Test location
    \begin{figure}[ht]
      \centering
      \includegraphics[width=0.6\textwidth]{faucon.png}
      \caption{faucon.png}
      \includegraphics[width=0.3\textwidth]{pix/faucon.jpg}
    \end{figure}
    \end{document}

## Generated figure {#generated-figure-7 .unnumbered}

Image file naming and path issues.

## Screenshot {#screenshot-7 .unnumbered}

::: center
![image](Naminggraphicsfiles.png){width="80%"}
:::

## Analysis {#analysis-7 .unnumbered}

This document demonstrates:

- Subdirectory path: `pix/faucon.jpg`

- Different image formats (.png, .jpg)

- Multiple images in same figure

------------------------------------------------------------------------

# Storinggraphicsinasubdirectory.tex - Graphics Path {#sec:graphicspath}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{graphicx}
    \graphicspath{{figs/}{pics/}}
    \begin{document}
    Test location
    \begin{figure}[ht]
      \centering
      \includegraphics[width=0.6\textwidth]{faucon.png}
      \caption{faucon.png}
    \end{figure}
    \end{document}

## Generated figure {#generated-figure-8 .unnumbered}

Setting graphics search path.

## Screenshot {#screenshot-8 .unnumbered}

::: center
![image](Storinggraphicsinasubdirectory.png){width="80%"}
:::

## Analysis {#analysis-8 .unnumbered}

This document demonstrates:

- `\graphicspath{{figs/}{pics/}}` to set search directories

- Organizing images in subdirectories

- Path specification syntax

------------------------------------------------------------------------

# Placingfloats.tex - Basic Float Placement {#sec:placing}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{graphicx}
    \begin{document}
    \begin{figure}[htbp]
      \centering
      \includegraphics[width=0.7\textwidth]{faucon.png}
      \caption{faucon.png}
    \end{figure}
    \end{document}

## Generated figure {#generated-figure-9 .unnumbered}

Basic float placement options.

## Screenshot {#screenshot-9 .unnumbered}

::: center
![image](Placingfloats.png){width="80%"}
:::

## Analysis {#analysis-9 .unnumbered}

This document demonstrates:

- Standard `figure` environment

- Placement specifier `[htbp]`

- `\centering` for alignment

- Caption with description

------------------------------------------------------------------------

# OtherTypesOfFlotTriv.tex - Custom Float Types {#sec:trivfloat2}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{graphicx}
    \newfloat{image}{htbp}{loi}
    \usepackage{float}
    \begin{document}
    \begin{image}
      \centering
      \includegraphics[width=0.7\textwidth]{faucon.png}
      \caption{faucon.png}
    \end{image}
    \begin{image}
     \centering
     \includegraphics[width=0.7\textwidth]{corbeau.jpg}
     \caption{corbeau.jpg}
    \end{image}
    \end{document}

## Generated figure {#generated-figure-10 .unnumbered}

Custom float types.

## Screenshot {#screenshot-10 .unnumbered}

::: center
![image](OtherTypesOfFlotTriv.png){width="80%"}
:::

## Analysis {#analysis-10 .unnumbered}

This document demonstrates:

- Custom float type `image`

- `\centering` for alignment

- Sequential caption numbering

- Different image formats in same float type

------------------------------------------------------------------------

# Conclusion: Methodology for Graphics and Floats {#conclusion-methodology-for-graphics-and-floats .unnumbered}

After comprehensive analysis of graphics and float examples, here is the
structured methodology for effectively including images and managing
floats in LaTeX:

## 1. Essential graphics inclusion structure {#essential-graphics-inclusion-structure .unnumbered}

    \documentclass{article}
    \usepackage{graphicx}        % Required for images

    \begin{document}
    % Basic image inclusion
    \includegraphics[width=0.5\textwidth]{image.jpg}

    % Figure float with caption
    \begin{figure}[htbp]
      \centering
      \includegraphics[height=5cm]{image.png}
      \caption{Description of image}
      \label{fig:label}
    \end{figure}

    % Cross-reference to figure
    As shown in Figure~\ref{fig:label}...
    \end{document}

## 2. Key commands and options {#key-commands-and-options .unnumbered}

  **Command/Option**   **Syntax**                          **Purpose**
  -------------------- ----------------------------------- ------------------------------
  \\includegraphics    `\includegraphics[keyvals]{file}`   Include image with options
  Width option         `width=0.5\textwidth`               Scale relative to text width
  Height option        `height=5cm`                        Set fixed height
  Scale option         `scale=0.75`                        Scale factor
  Trim/Clip            `clip, trim= l b r t`               Crop image edges
  Graphics path        `\graphicspath{{subdir/}}`          Set search directories
  \\caption            `\caption{text}`                    Add caption to float
  \\label              `\label{fig:name}`                  Mark for referencing
  \\ref                `\ref{fig:name}`                    Reference by number

## 3. Float placement specifiers {#float-placement-specifiers .unnumbered}

  **Specifier**   **Meaning**
  --------------- ------------------------------------------------
  h               Here - approximately at this point in the text
  t               Top - at the top of a page
  b               Bottom - at the bottom of a page
  p               Page - on a separate float page
  !               Override - ignore certain restrictions
