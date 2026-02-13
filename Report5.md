# 1ManipulatingThespaceBetweenColumns - Column Spacing {#sec:colspace}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{array}
    \setlength\tabcolsep{1cm}

    \begin{document}
    \section{Introduction to space between columns}
    This space is defined with the length \verb|\tabcolsep|. Due
    to the fact that each column is padded on both sides you get one \verb|\tabcolsep|
    on either end of the table, and 2 \verb|\tabcolsep| between two columns one from each
    column. We can adjust this space to any length using  \verb|\setlength|.

    \begin{tabular}{lll}
      Animal & Food   & Size   \\
      dog    & meat   & medium \\
      horse  & hay    & large  \\
      frog   & flies  & small  \\
    \end{tabular}
    \end{document}

## Generated figure {#generated-figure .unnumbered}

Table with increased column spacing (1cm).

## Screenshot {#screenshot .unnumbered}

::: center
![image](1ManipulatingThespaceBetweenColumns.png){width="80%"}
:::

------------------------------------------------------------------------

# 2ndNumericAlignmentInColumns - Numeric Alignment {#sec:numeric}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{booktabs}
    \usepackage{siunitx}
    \begin{document}

    \section{Commentary and Interpretation}
    Here I just try one eg in: package documentation Page 5,
     Titre: 3.1 Numbers

    \begin{tabular}{SS}
    \toprule
    {Values} &   {More Values} \\
    \midrule
    123           &      \num{123}     \\
    1234           &      \num{1234}    \\
    12345            &      \num{12345}   \\
    0.123           &      \num{0.123}   \\
    0,1234           &      \num{0,1234}  \\
    0.12345            &      \num{.12345}  \\
    \bottomrule
    \end{tabular}
    \end{document}

## Generated figure {#generated-figure-1 .unnumbered}

Numeric alignment with siunitx package.

## Screenshot {#screenshot-1 .unnumbered}

::: center
![image](2ndNumericAlignmentInColumns.png){width="80%"}
:::

------------------------------------------------------------------------

# 51TheArrayPackage - Basic Array Usage {#sec:51}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{array}
    \begin{document}
    \section{Array}
    \begin{tabular}{lll}
      Animal  & Food  &  Size   \\
      dog     & meat  & medium  \\
      horse   & hay   & large   \\
      frog    & flies & small   \\
    \end{tabular}

    \section{My intepretation}
    ~We can see three (03) Columns (Animals, Foods and Size) because of using Array Package: {array}

    ~To succed this compillation we have to use at the begin (111 = '3' the number of the Column){tabular} 
    but at the end we have To use {tabular}.
    \end{document}

## Generated figure {#generated-figure-2 .unnumbered}

Basic table with three columns.

## Screenshot {#screenshot-2 .unnumbered}

::: center
![image](51TheArrayPackage.png){width="80%"}
:::

------------------------------------------------------------------------

# 52TheArrayPackageALotOfText - Long Text in Columns {#sec:52}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{array}

    \begin{document}

    \section{Trying the type l.}

    We will see 2 Columns (c=Animal and l=left aligned column=Description) because of the use of: {tabular}{cl}
    \section{Array:2}
    \begin{tabular}{cl}
      Animal  & Description \\
      dog     & The dog is a member of the genus Canis,which forms part of the
                wolf-like canids, and is the most widely abundant terrestrial carnivore. \\
    cat       & The cat is a domestic species of small carnivorous mammal. It is the 
                only domesticated species in the family Felidae and is often referred 
                to as the domestic cat to distinguish it from the wild members of the
                family. \\
    \end{tabular}

    \section{My intepretation}
    Here the issue is that the l type column typesets its contents in a single row at its natural
    width, even if there is a page border in the way.But we can correcte it.
    \end{document}

## Generated figure {#generated-figure-3 .unnumbered}

Table with long text in left-aligned column.

## Screenshot {#screenshot-3 .unnumbered}

::: center
![image](52TheArrayPackageALotOfText.png){width="80%"}
:::

------------------------------------------------------------------------

# 53TheArrayPackageALotOfTextTypeCP - Paragraph Columns (9cm) {#sec:53}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{array}

    \begin{document}

    \section{Trying the type cp: {9cm.}}

    We will see 2 Columns (c=Animal and p=column fully justified=Description) because of the use of: {tabular}{cp}
    \section{Array:2}
    \begin{tabular}{cp{9cm}} % We are going to use "cp" to justifie the text
      Animal  & Description \\
      dog     & The dog is a member of the genus Canis, which forms
          part of the
              wolf-like canids, and is the most widely abundant
                terrestrial
              carnivore. \\
      cat     & The cat is a domestic species of small carnivorous
         mammal. It is the
              only domesticated species in the family Felidae and
                is often referred
              to as the domestic cat to distinguish it from the
                 wild members of the
              family. \\
    \end{tabular}

    \section{My intepretation}
    Here the text will be
    automatically line wrapped and fully justified
    m{9cm} like p, but vertically centered compared to the rest of the
    row.
    will try for 5cm and see in the next file.
    \end{document}

## Generated figure {#generated-figure-4 .unnumbered}

Table with paragraph column (9cm width).

## Screenshot {#screenshot-4 .unnumbered}

::: center
![image](53TheArrayPackageALotOfTextTypeCP.png){width="80%"}
:::

------------------------------------------------------------------------

# 53TheArrayPackageALotOfTextTypeCP5 - Paragraph Columns (5cm) {#sec:53-5}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{array}

    \begin{document}

    \section{Trying the type cp: {5cm.}}

    We will see 2 Columns (c=Animal and p=column fully justified=Description) because of the use of: {tabular}{cp}
    \section{Array:2}
    \begin{tabular}{cp{5cm}} % My own Eg to make justification between 5cm
      Animal  & Description \\
      dog     & The dog is a member of the genus Canis, which forms
          part of the
              wolf-like canids, and is the most widely abundant
                 terrestrial
              carnivore. \\
      cat     & The cat is a domestic species of small carnivorous
         mammal. It is the
              only domesticated species in the family Felidae and
                 is often referred
              to as the domestic cat to distinguish it from the
                 wild members of the
              family. \\
    \end{tabular}

    \section{My intepretation}
    Here the text will be
    automatically line wrapped and fully justified
    m{5cm} like p, but vertically centered compared to the rest of the
    row.
    Here We  can see for 5cm.
    \end{document}

## Generated figure {#generated-figure-5 .unnumbered}

Table with narrower paragraph column (5cm width).

## Screenshot {#screenshot-5 .unnumbered}

::: center
![image](53TheArrayPackageALotOfTextTypeCP5.png){width="80%"}
:::

------------------------------------------------------------------------

# 54TheArrayPackageTheSameType - Multiple Same Type Columns {#sec:54}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{array}

    \begin{document}

    \section{Trying the type cp:{6}{c} the same type}

    We will see 2 Columns: c=Animal and p=column fully justified=Description,
    because of the use of: \verb|{tabular}{6}{c}| same type.
    \section{Array:2}
    \begin{tabular}{6}{c} 
      Animal  & Description \\
      dog     & The dog is a member of the genus Canis, which forms
          part of the
              wolf-like canids, and is the most widely abundant
                terrestrial
              carnivore. \\
      cat     & The cat is a domestic species of small carnivorous
         mammal. It is the
              only domesticated species in the family Felidae and
                is often referred
              to as the domestic cat to distinguish it from the
                 wild members of the
              family. \\
    \end{tabular}

    \section{My intepretation}
    Here the text will be
    automatically line wrapped and fully justified
    m{6cm} like p, but vertically centered compared to the rest of the
    row.And at the end the number of table has many columns of the same type.
    Here We  can see for {6}{c}cm.
    \end{document}

## Generated figure {#generated-figure-6 .unnumbered}

Table with multiple same-type columns (error demonstration).

## Screenshot {#screenshot-6 .unnumbered}

::: center
![image](54TheArrayPackageTheSameType.png){width="80%"}
:::

------------------------------------------------------------------------

# 541TheArrayPackageEquivalC - Using \*ntype Syntax {#sec:541}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{array}
    \begin{document}

    \begin{tabular}{*{3}{l}}
      Animal & Food  & Size    \\
      dog    & meat  & medium  \\
      horse  & hay   & large   \\
      frog   & flies & small   \\
    \end{tabular}
    \end{document}

## Generated figure {#generated-figure-7 .unnumbered}

Table with \*3l syntax for three left-aligned columns.

## Screenshot {#screenshot-7 .unnumbered}

::: center
![image](541TheArrayPackageEquivalC.png){width="80%"}
:::

------------------------------------------------------------------------

# 55AddingRulesLines - Basic Table Rules {#sec:55}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{array}
    \usepackage{booktabs}

    \begin{document}

    \section{Different types of lines:toprule, midrule, and bottomrule}

    \begin{tabular}{lll}
      \toprule
      Animal & Food & Size \\
      \midrule
      dog    & meat  & medium  \\
      horse  & hay   & large   \\
      frog   & flies & small   \\ 
      \bottomrule
    \end{tabular}

    section{My commentary:}
    The use of these keys(toprule, midrule, and bottomrule) gives us the possibility to get 
    \end{document}

## Generated figure {#generated-figure-8 .unnumbered}

Table with booktabs rules (toprule, midrule, bottomrule).

## Screenshot {#screenshot-8 .unnumbered}

::: center
![image](55AddingRulesLines.png){width="80%"}
:::

------------------------------------------------------------------------

# 55AddingRulesLines1 - cmidrule Usage {#sec:55-1}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{array}
    \usepackage{booktabs}

    \begin{document}
    The fourth rule command provided by booktabs is \verb|\cmidrule|. It can be used
    to draw a rule that doesn't span the entire width of the table but only a specified
    column range. A column range is entered as a number span: {number-number}.
    \begin{tabular}{lll}
      \toprule
     Animal & Food & Size \\
      \midrule
      dog & meat & medium \\
      \cmidrule{1-2}
      horse & hay & large \\
      \cmidrule{1-1}
      \cmidrule{3-3}
      frog & flies & small \\
      \bottomrule
    \end{tabular}
    \end{document}

## Generated figure {#generated-figure-9 .unnumbered}

Table with partial rules using cmidrule.

## Screenshot {#screenshot-9 .unnumbered}

::: center
![image](55AddingRulesLines1.png){width="80%"}
:::

------------------------------------------------------------------------

# 55AddingRulesLines2 - cmidrule with Trimming {#sec:55-2}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{array}
    \usepackage{booktabs}

    \begin{document}

    There is another useful feature of \verb|\cmidrule|.
    We can shorten it on either end
    with an optional argument enclosed in parentheses:
      \begin{tabular}{lll}
      \toprule
      Animal & Food & Size \\
      \midrule
      dog & meat & medium \\
      \cmidrule{1-2}
      horse & hay & large \\ 
      \cmidrule(r){1-1}
      \cmidrule(rl){2-2}
      \cmidrule(l){3-3}
      frog & flies & small \\
      \bottomrule
    \end{tabular}
    We may have guessed that r and l mean the rule is shortened on its right and left
    end, respectively
    \end{document}

## Generated figure {#generated-figure-10 .unnumbered}

Table with trimmed cmidrule rules.

## Screenshot {#screenshot-10 .unnumbered}

::: center
![image](55AddingRulesLines2.png){width="80%"}
:::

------------------------------------------------------------------------

# 55AddingRulesLines3 - addlinespace Usage {#sec:55-3}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{array}
    \usepackage{booktabs}

    \begin{document}

    \section{The meaning of booktabs:Rules Lines.}
    Sometimes a rule would be too much of a separation for two rows but to get across
    the meaning more clearly you want to separate them by some means. In this case
    we can use \\addlinespace to insert a small skip.
    \section{Animal and Description with the rules:}

    \begin{tabular}{cp{9cm}}
      \toprule
      Animal & Description \\
      \midrule
               dog & The dog is a member of the genus Canis, which forms part of the
               wolf-like canids, and is the most widely abundant terrestrial carnivore. \\
      \addlinespace
               cat & The cat is a domestic species of small carnivorous mammal. It is the
               only domesticated species in the family Felidae and
                  is often referred
               to as the domestic cat to distinguish it from the
                  wild members of the
               family. \\
      \bottomrule
    \end{tabular}
    \end{document}

## Generated figure {#generated-figure-11 .unnumbered}

Table with vertical spacing using addlinespace.

## Screenshot {#screenshot-11 .unnumbered}

::: center
![image](55AddingRulesLines3.png){width="80%"}
:::

------------------------------------------------------------------------

# 56MergingCells - Horizontal Cell Merging {#sec:56}

    \documentclass{article}
    \usepackage{array, booktabs}

    \begin{document}

    \begin{tabular}{lcc}
    \toprule
    \multicolumn{1}{c}{Animal} & Taille & Poids \\
    \midrule
    Chien & Moyen & 15 kg \\
    Chat & Petit & 5 kg \\
    Éléphant & Grand & 5000 kg \\
    \bottomrule
    \end{tabular}

    \bigskip

    % Tableau avec fusion horizontale
    \begin{tabular}{|l|c|c|}
    \hline
    \multicolumn{3}{|c|}{Informations} \\
    \hline
    Nom & Âge & Ville \\
    \hline
    Alice & 25 & Paris \\
    Bob & 30 & Londres \\
    \hline
    \end{tabular}

    \end{document}

## Generated figure {#generated-figure-12 .unnumbered}

Tables with horizontally merged cells using multicolumn.

## Screenshot {#screenshot-12 .unnumbered}

::: center
![image](56MergingCells.png){width="80%"}
:::

------------------------------------------------------------------------

# 56MergingCells2 - Vertical Merging Simulation {#sec:56-2}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{array}
    \usepackage{booktabs}

    \begin{document}
    \section{Explication}
    Merging cells vertically isn't supported by LaTeX. Usually it suffices to leave cells
    empty to give the reader the correct idea of what was meant without explicitly
    making cells span rows.

    \begin{tabular}{lll}
     \toprule
     Group & Animal & Size \\
     \midrule
     herbivore & horse & large \\
               & deer & medium \\
               & rabbit & small \\
     \addlinespace
     carnivore & dog & medium \\
               & cat & small \\
               & lion & large \\
     \addlinespace
     omnivore  & crow & small \\
               & bear & large \\
               & pig & medium \\
     \bottomrule
     \end{tabular}
    \end{document}

## Generated figure {#generated-figure-13 .unnumbered}

Table simulating vertical merging with empty cells.

## Screenshot {#screenshot-13 .unnumbered}

::: center
![image](56MergingCells2.png){width="80%"}
:::

------------------------------------------------------------------------

# 571StylingAColumn - Column Styling {#sec:571}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{array}
    \usepackage{booktabs}
    \begin{document}
    \begin{tabular}{>{\itshape}l<{:} *{2}{l}}
      \toprule
      Animal & Food & Size \\
      \midrule
      dog & meat & medium \\
      horse & hay & large \\
      frog & flies & small \\
      \bottomrule
    \end{tabular}
    \end{document}

## Generated figure {#generated-figure-14 .unnumbered}

Table with italic first column and colon separator.

## Screenshot {#screenshot-14 .unnumbered}

::: center
![image](571StylingAColumn.png){width="80%"}
:::

------------------------------------------------------------------------

# 572StylingAColumn - Header Exclusion from Styling {#sec:572}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{array}
    \usepackage{booktabs}

    \begin{document}
    \begin{tabular}{>{\itshape}l<{:} *{2}{l}}
      \toprule
      \multicolumn{1}{l}{Animal} & Food & Size \\
      \midrule
      dog & meat & medium \\
      horse & hay & large \\
      frog & flies & small \\
      \bottomrule

    We may want the first cell not to be affected because it is the table head.
    Here \\multicolumn may be used
    \end{tabular}
    \end{document}

## Generated figure {#generated-figure-15 .unnumbered}

Table with header excluded from column styling.

## Screenshot {#screenshot-15 .unnumbered}

::: center
![image](572StylingAColumn.png){width="80%"}
:::

------------------------------------------------------------------------

# 573StylingAColumn - @\... Syntax {#sec:573}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{array}
    \begin{document}
    \begin{tabular}{l@{ : }l@{\hspace{2cm}}l}
      Animal & Food & Size \\
      dog & meat & medium \\
      horse & hay & large \\
      frog & flies & small \\

    section{Commentary:}
    This preamble token does something pretty similar. The difference is, that it adds
    its argument in center of the space between two columns.  
    \end{tabular}
    \end{document}

## Generated figure {#generated-figure-16 .unnumbered}

Table with custom column separators.

## Screenshot {#screenshot-16 .unnumbered}

::: center
![image](573StylingAColumn.png){width="80%"}
:::

------------------------------------------------------------------------

# 581StylingAColumnvertical - Vertical Rules {#sec:581}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{array}

    \begin{document}
    \begin{tabular}{l|ll}
      Animal & Food  & Size   \\[2pt]
      dog    & meat  & medium \\
      horse  & hay   & large  \\
      frog   & flies & small  \\
    \end{tabular}
    \section{Intepretation}: We might notice that the behavior of this implementation is pretty similar to \\{decl}; it adds the
    vertical rule between two columns leaving the padding as it is.
    \end{document}

## Generated figure {#generated-figure-17 .unnumbered}

Table with vertical rule and row spacing.

## Screenshot {#screenshot-17 .unnumbered}

::: center
![image](581StylingAColumnvertical.png){width="80%"}
:::

------------------------------------------------------------------------

# 591CustomizingRooktabsRules - Custom Rule Thickness {#sec:591}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{array}
    \usepackage{booktabs}

    \begin{document}

     \begin{tabular}{@{} lll@{}} \toprule[2pt]
       Animal & Food & Size \\ \midrule[1pt]
       dog & meat & medium \\
       \cmidrule[0.5pt](r{1pt}l{1cm}){1-2}
       horse & hay & large \\
       frog & flies & small \\ \bottomrule[2pt]
    \end{tabular}
    \end{document}

## Generated figure {#generated-figure-18 .unnumbered}

Table with customized rule thickness.

## Screenshot {#screenshot-18 .unnumbered}

::: center
![image](591CustomizingRooktabsRules.png){width="80%"}
:::

------------------------------------------------------------------------

# 600NumericAlignmentInColumns - Numeric Alignment with siunitx {#sec:600}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{booktabs}
    \usepackage{siunitx}
    \begin{document}
    \begin{tabular}{SS}
    \toprule
    {Values} &   {More Values} \\
    \midrule
    1        &    2.3456 \\
    1.2      &    34.2345 \\
    -2.3     &    90.473 \\
    40       &    5642.5 \\
    5.3      &    1.2e3 \\
    0.2      &    1e4 \\
    \bottomrule
    \end{tabular}
    \section{Commentary and Interpretation}
    Here, before succeed to run the file,
    i was oblige to install the paquets siunitx.
    \end{document}

## Generated figure {#generated-figure-19 .unnumbered}

Table with numeric alignment using siunitx S columns.

## Screenshot {#screenshot-19 .unnumbered}

::: center
![image](600NumericAlignmentInColumns.png){width="80%"}
:::

------------------------------------------------------------------------

# 601SpecifyingTotalTableWidthtabularx - tabularx Environment {#sec:601x}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{tabularx}
    \begin{document}

    The tabularx environment, provided by the package of the same name, has a
    similar syntax to tabular* but instead of adjusting the inter-column space, adjusts
    the widths of columns specified by a new column type, X. This is equivalent to a
    specification of p{...} for an automatically determined width.

    \begin{center}
    \begin{tabular}{lp{2cm}}
    \hline
    A & B B B B B B B B B B B B B B B B B B B B B B B B\\
    C & D D D D D D D\\
    \hline
    \end{tabular}
    \end{center}
    \begin{center}
    \begin{tabularx}{.5\textwidth}{lX}
    \hline
    A & B B B B B B B B B B B B B B B B B B B B B B B B\\
    C & D D D D D D D\\
    \hline
    \end{tabularx}

    \end{center}
    \begin{center}
    \begin{tabularx}{\textwidth}{lX}
    \hline
    A & B B B B B B B B B B B B B B B B B B B B B B B B\\
    C & D D D D D D D\\
    \hline
    \end{tabularx}
    \end{center}
    \section{Commentary and intepretation} 
      The tabularx environment, provided by the package of the same name, has a
    similar syntax to tabular* but instead of adjusting the inter-column space, adjusts
    the widths of columns specified by a new column type, X. This is equivalent to a
    specification of p{...} for an automatically determined width.
    \section{Conlusion}
    Unlike the other forms discussed in these lessons, tabularx needs to typeset the
    table several times with trial widths to determine the final setting. This means
    that there are several restrictions on the use of the environment; We can see the package
    documentation to learn about its.
    \end{document}

## Generated figure {#generated-figure-20 .unnumbered}

Tables demonstrating tabularx with X columns.

## Screenshot {#screenshot-20 .unnumbered}

::: center
![image](601SpecifyingTotalTableWidthtabularx.png){width="80%"}
:::

------------------------------------------------------------------------

# 602MultiPagesTableNotes - Table with Notes {#sec:602notes}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{array}
    \usepackage{threeparttable}
    \begin{document}

    \begin{table}
    \begin{threeparttable}
       \caption{An Example}
       \begin{tabular}{ll}
        An entry & 42\tnote{1}\\
        Another entry & 24\tnote{2}\\
       \end{tabular}
       \begin{tablenotes}
       \item [1] the first note.
       \item [2] the second note.
       \end{tablenotes}
    \end{threeparttable}
    \end{table}
    \end{document}

## Generated figure {#generated-figure-21 .unnumbered}

Table with footnotes using threeparttable.

## Screenshot {#screenshot-21 .unnumbered}

::: center
![image](602MultiPagesTableNotes.png){width="80%"}
:::

------------------------------------------------------------------------

# 602Multi-PageTablesLongtablePackage - Longtable Example {#sec:602long}

    \documentclass{article}
    \usepackage[paperheight=8cm,paperwidth=8cm]{geometry}
    \usepackage{array}
    \usepackage{longtable}
    \begin{document}

    \begin{longtable}{cc}
    \caption{A Long Table} \\
    Left Side & Right Side\\
    \hline
    \endfirsthead

    \multicolumn{2}{c}{\tablename\ \thetable\ (continued)} \\
    Left Side & Right Side\\
    \hline
    \endhead

    \hline
    \endfoot
    \hline
    \endlastfoot

    aa & bb\\
    Entry & b\\
    a & b\\
    a & b\\
    a & b\\
    a & b\\
    a & b\\
    a & bbb\\
    a & b\\
    a & b\\
    a & b\\
    a & b\\
    a & b\\
    a & b\\
    a & b b b b b b\\
    a & b b b b b\\
    a & b b\\
    A Wider Entry & b\\
    \end{longtable}

    \end{document}

## Generated figure {#generated-figure-22 .unnumbered}

Multi-page table using longtable package.

## Screenshot {#screenshot-22 .unnumbered}

::: center
![image](602Multi-PageTablesLongtablePackage.png){width="80%"}
:::

------------------------------------------------------------------------

# 603TypesettingInNarrowColumns - Text in Narrow Columns {#sec:603}

    \documentclass[a4paper]{article}
    \usepackage[T1]{fontenc}
    \usepackage{array}
    \usepackage{ragged2e}
    \begin{document}

    \begin{table}
        
    \begin{tabular}[t]{lp{3cm}}
    One & A long text set in a narrow paragraph, with some more
       example text.\\
    Two & A different long text set in a narrow paragraph, with
       some more hard to hyphenate words.
    \end{tabular}%
    \begin{tabular}[t]{l>{\raggedright\arraybackslash}p{3cm}}
    One & A long text set in a narrow paragraph, with some more
       example text.\\
    Two & A different long text set in a narrow paragraph, with
       some more hard to hyphenate words.
    \end{tabular}%
    \begin{tabular}[t]{l>{\RaggedRight}p{3cm}}
    One & A long text set in a narrow paragraph, with some more
       example text.\\
    Two & A different long text set in a narrow paragraph, with
       some more hard to hyphenate words.
    \end{tabular}
    \footnotesize
    \begin{tabular}[t]{lp{3cm}}
    One & A long text set in a narrow paragraph, with some more
       example text.\\
    Two & A different long text set in a narrow paragraph, with
       some more hard to hyphenate words.
    \end{tabular}

    \end{table}

    \end{document}

## Generated figure {#generated-figure-23 .unnumbered}

Tables with text in narrow columns and different text alignment.

## Screenshot {#screenshot-23 .unnumbered}

::: center
![image](603TypesettingInNarrowColumns.png){width="80%"}
:::

------------------------------------------------------------------------

# 605ControlVerticalTricks - Vertical Alignment Control {#sec:605}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{array}
    \usepackage{booktabs}

    \begin{document}
    \begin{tabular}{lcc}
      \toprule
      Test & \begin{tabular}[b]{@{}c@{}}A\\a\end{tabular} &
         \begin{tabular}[t]{@{}c@{}}B\\b\end{tabular} \\
      \midrule
      Content & is & here \\
      Content & is & here \\
      Content & is & here \\
      \bottomrule
    \end{tabular}
    We Note that We can control vertical alignment by an optional argument to the tabular;
    it supports the usage of t, c, or b for top, centered,or bottom aligned respectively.

    \end{document}

## Generated figure {#generated-figure-24 .unnumbered}

Table with nested tables demonstrating vertical alignment.

## Screenshot {#screenshot-24 .unnumbered}

::: center
![image](605ControlVerticalTricks.png){width="80%"}
:::

------------------------------------------------------------------------

# 605VerticalTricks - Nested Tables {#sec:605v}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{array}
    \usepackage{booktabs}

    \begin{document}
    \begin{tabular}{lcc}
      \toprule
      Test & \begin{tabular}{@{}c@{}}A\\a\end{tabular} &
             \begin{tabular}{@{}c@{}}B\\b\end{tabular} \\
      \midrule
      Content & is & here \\
      Content & is & here \\
      Content & is & here \\
      \bottomrule
    \end{tabular}
    \end{document}

## Generated figure {#generated-figure-25 .unnumbered}

Table with centered nested tables.

## Screenshot {#screenshot-25 .unnumbered}

::: center
![image](605VerticalTricks.png){width="80%"}
:::

------------------------------------------------------------------------

# 606LineSpacingInTables - Line Spacing Control {#sec:606}

    \documentclass[a4paper]{article}
    \usepackage[T1]{fontenc}
    \usepackage{array}
    \begin{document}

    \begin{center}
    \begin{tabular}{cc}
    \hline
    Square& $x^2$\\
    \hline
    Cube& $x^3$\\
    \hline
    \end{tabular}
    \end{center}

    \begin{center}
    \setlength\extrarowheight{2pt}
    \begin{tabular}{cc}
    \hline
    Square& $x^2$\\
    \hline
    Cube& $x^3$\\
    \hline
    \end{tabular}
    \end{center}
    \end{document}

## Generated figure {#generated-figure-26 .unnumbered}

Tables demonstrating line spacing control with extrarowheight.

## Screenshot {#screenshot-26 .unnumbered}

::: center
![image](606LineSpacingInTables.png){width="80%"}
:::

------------------------------------------------------------------------

# 601SpecifyingTotalTableWidthtabular - Fixed Width Tables {#sec:601}

    \documentclass{article}
    \usepackage[T1]{fontenc}
    \usepackage{array}
    \begin{document}

    \begin{center}
    \begin{tabular}{cc}
    \hline
    A & B\\
    C & D\\
    \hline
    \end{tabular}
    \end{center}

    \begin{center}
    \begin{tabular*}{.5\textwidth}{@{\extracolsep{\fill}}cc@{}}
    \hline
    A & B\\
    C & D\\
    \hline
    \end{tabular*}

    \end{center}
    \begin{center}
    \begin{tabular*}{\textwidth}{@{\extracolsep{\fill}}cc@{}}
    \hline
    A & B\\
    C & D\\
    \hline
    \end{tabular*}
    \end{center}
    \ The tabular* environment takes an additional width argument that specifies
    the total width of the table. Stretchy space must be added to the table 
    using the \verb|\extracolsep| command. This space is added between all columns from that
    point in the preamble. It is almost always used with \verb|\fill| a special space that
    stretches to be as large as necessary
    \end{document}

## Generated figure {#generated-figure-27 .unnumbered}

Tables with specified total width using tabular\*.

## Screenshot {#screenshot-27 .unnumbered}

::: center
![image](601SpecifyingTotalTableWidthtabular.png){width="80%"}
:::

------------------------------------------------------------------------

# Conclusion: Methodology for Creating Tables {#conclusion-methodology-for-creating-tables .unnumbered}

After comprehensive analysis of table examples, here is the structured
methodology for creating effective tables:

## 1. Essential table structure {#essential-table-structure .unnumbered}

    \begin{tabular}{column specifications}
      \toprule
      Header1 & Header2 & Header3 \\
      \midrule
      Data1   & Data2   & Data3   \\
      Data4   & Data5   & Data6   \\
      \bottomrule
    \end{tabular}

## 2. Column type specifications {#column-type-specifications .unnumbered}

  **Type**   **Description**               **Use Case**
  ---------- ----------------------------- --------------------------------------
  l          Left-aligned column           Text data, labels
  c          Centered column               Numbers, short text
  r          Right-aligned column          Numbers, dates
  p{width}   Paragraph column              Long text, descriptions
  m{width}   Middle-aligned paragraph      Text with vertical centering
  b{width}   Bottom-aligned paragraph      Special layouts
  S          Numeric alignment (siunitx)   Decimal numbers, scientific notation
  X          Automatic width (tabularx)    Flexible column widths

## 3. Recommended workflow {#recommended-workflow .unnumbered}

**Step 1: Plan table structure**

- Determine number of columns and rows

- Choose appropriate column types

- Consider table width and alignment

**Step 2: Create basic table**

1.  Set up tabular environment with column specifications

2.  Add headers

3.  Insert data rows

**Step 3: Enhance appearance**

- Add rules (toprule, midrule, bottomrule, cmidrule)

- Adjust column spacing (tabcolsep)

- Style columns (\>, \<, @)

- Add vertical spacing (addlinespace, \[dim\])

**Step 4: Test and refine**

- Check width and alignment

- Verify readability

- Test with different data

## 4. Advanced techniques {#advanced-techniques .unnumbered}

::: framed
**Key advanced features:**

1\. **Multi-column cells**: `\multicolumn{n}{type}{content}`

2\. **Column styling**: `>{\itshape}l` for italic first column

3\. **Custom separators**: `@{ : }` for colon separator

4\. **Fixed width tables**: `tabular*` with `\extracolsep{\fill}`

5\. **Vertical alignment**: Optional argument `[t]`, `[c]`, `[b]` to
tabular

6\. **Numeric formatting**: siunitx package for decimal alignment

7\. **Multi-page tables**: longtable package for tables spanning pages

8\. **Table notes**: threeparttable package for footnotes
:::

## 5. Best practices {#best-practices .unnumbered}

  **Practice**                    **Benefit**
  ------------------------------- -----------------------------------------
  Use booktabs for rules          Professional appearance, proper spacing
  Consistent alignment            Improved readability
  Appropriate column widths       Balanced layout
  Minimal vertical rules          Clean, modern look
  Proper header styling           Clear data organization
  Adequate spacing                Easy to read and interpret
  Use X columns for flexibility   Automatic width adjustment

## 6. Common issues and solutions {#common-issues-and-solutions .unnumbered}

- **Overfull hboxes**: Adjust column widths or use tabularx

- **Poor text wrapping**: Use p{width} column type or ragged2e

- **Uneven spacing**: Adjust tabcolsep or use @ syntax

- **Vertical alignment issues**: Use m{width} or vertical position
  optional argument

- **Decimal misalignment**: Use siunitx S column type

- **Multi-page tables**: Use longtable instead of tabular

- **Table notes**: Use threeparttable for proper footnote placement

**Final recommendation**: Start with simple tables using basic column
types, gradually incorporate advanced features as needed, and always
prioritize clarity and readability. Well-designed tables effectively
communicate complex data and enhance document professionalism.
