# Installing TeX Live - General Information {#sec:general}

    Installing the distribution TeXlive.

    1.1.1 General information
    • TeXLive - the most complete LaTeX distribution supported by the TeX community.
    • Supports a large number of operating systems.
    • Developed since 1996.
    • Based on the teTeX distribution.
    • MacTeX - a variant for MacOS.
    • Main page: https://www.tug.org/texlive/
    • TeXLive is a distribution with continuous updates as part of the annual
      version of the distribution.

## Generated figure (simulation) {#generated-figure-simulation .unnumbered}

General information about TeX Live distribution.

## Screenshot {#screenshot .unnumbered}

::: center
![image](texlive-full-install-progress.png){width="80%"}
:::

## Key Information Summary {#key-information-summary .unnumbered}

  **Feature**         **Description**
  ------------------- -------------------------------------
  Distribution Name   TeX Live
  Type                Complete LaTeX distribution
  First Release       1996
  Based on            teTeX distribution
  Mac Variant         MacTeX
  Official Website    `https://www.tug.org/texlive/`
  Update Model        Continuous updates, annual releases

------------------------------------------------------------------------

# Installation from Distribution Packages {#sec:packages}

    1.1.2 Installation from distribution packages
    • Ubuntu:
      apt install texlive-full
    • Windows. Use the Chocolatey package manager.
      choco install texlive

## Generated figure (simulation) {#generated-figure-simulation-1 .unnumbered}

Package manager installation commands.

## Screenshot - Chocolatey Installation {#screenshot---chocolatey-installation .unnumbered}

::: center
![image](chocolatey-install-powershell.png){width="80%"}
:::

## Screenshot - Chocolatey Success {#screenshot---chocolatey-success .unnumbered}

::: center
![image](chocolatey-install-success.png){width="80%"}
:::

## Installation Commands {#installation-commands .unnumbered}

::: framed
**Ubuntu/Debian (Linux):**

    sudo apt update
    sudo apt install texlive-full

**Windows (with Chocolatey):**

    choco install texlive

**Note:** The `texlive-full` package installs the complete TeX Live
distribution including all packages, fonts, and documentation. This can
take significant disk space (several gigabytes) and time to download.
:::

## Advantages of Package Manager Installation {#advantages-of-package-manager-installation .unnumbered}

- Easy installation with single command

- Automatic dependency resolution

- Integrated with system package management

- Easy updates via system package manager

## Disadvantages {#disadvantages .unnumbered}

- May not be the latest version

- Limited to distribution's repository version

- Less control over installation components

------------------------------------------------------------------------

# Manual Installation - Unix/Linux {#sec:manual-unix}

    1.1.3 Manual installation
    • Links on the site are to mirrors. The mirror is selected automatically.
    • Download the installer:
      • Unix: https://mirror.ctan.org/systems/texlive/tlnet/install-tl-unx.tar.gz
      
      cd /tmp/
      wget https://mirror.ctan.org/systems/texlive/tlnet/install-tl-unx.tar.gz

    • For Linux
      • Unpack the downloaded file:
        tar xzvf install-tl-unx.tar.gz
      • Go to the unpacked directory and run the installer:
        cd install-tl-[0-9]*
        sudo ./install-tl
      • It is recommended to create links to executable files in the /usr/local/bin
        directory. To do this, in the console version of the utility, select the O option,
        and then L. To return to the previous menu, use R.

## Generated figure (simulation) {#generated-figure-simulation-2 .unnumbered}

Manual installation process for Unix/Linux systems.

## Screenshot {#screenshot-1 .unnumbered}

::: center
![image](texlive-install-beginning.png){width="80%"}
:::

## Step-by-Step Installation Guide {#step-by-step-installation-guide .unnumbered}

::: framed
**Complete Unix/Linux Installation Procedure:**

1\. **Download the installer:**

    cd /tmp/
    wget https://mirror.ctan.org/systems/texlive/tlnet/install-tl-unx.tar.gz

2\. **Extract the archive:**

    tar xzvf install-tl-unx.tar.gz

3\. **Navigate to the installer directory:**

    cd install-tl-*

4\. **Run the installer with root privileges:**

    sudo ./install-tl

5\. **Configure installation options (optional):**

- Select `O` for options menu

- Select `L` to create symbolic links in `/usr/local/bin`

- Press `R` to return to previous menu

- Press `I` to begin installation
:::

## Installation Options Explained {#installation-options-explained .unnumbered}

  **Option**   **Description**
  ------------ ----------------------------------------------
  O            Opens options menu for configuration
  L            Creates symbolic links in system directories
  R            Returns to previous menu
  I            Starts the installation process

------------------------------------------------------------------------

# Manual Installation - Windows {#sec:manual-windows}

    • Windows: https://mirror.ctan.org/systems/texlive/tlnet/install-tl-windows.exe
    • For Windows: run the executable file and install.

## Generated figure (simulation) {#generated-figure-simulation-3 .unnumbered}

Windows installer executable.

## Screenshot - Installation Progress 1 {#screenshot---installation-progress-1 .unnumbered}

::: center
![image](texlive-install-progress-1.png){width="80%"}
:::

## Screenshot - Installation Progress 2 {#screenshot---installation-progress-2 .unnumbered}

::: center
![image](texlive-install-progress-2.png){width="80%"}
:::

## Screenshot - Installation Progress 3 {#screenshot---installation-progress-3 .unnumbered}

::: center
![image](texlive-install-progress-3.png){width="80%"}
:::

## Screenshot - Installation Completion {#screenshot---installation-completion .unnumbered}

::: center
![image](texlive-install-completion.png){width="80%"}
:::

## Windows Installation Guide {#windows-installation-guide .unnumbered}

::: framed
**Windows Installation Steps:**

1\. **Download the installer:**

- Visit:
  `https://mirror.ctan.org/systems/texlive/tlnet/install-tl-windows.exe`

- Or use the direct link:
  `https://mirror.ctan.org/systems/texlive/tlnet/install-tl-windows.exe`

2\. **Run the installer:**

- Double-click the downloaded `install-tl-windows.exe` file

- Allow administrator privileges if prompted

3\. **Follow the installation wizard:**

- Choose installation directory (default: `C:\texlive\[year]`)

- Select installation scheme (recommended: full installation)

- Choose whether to create shortcuts

- Click \"Install\" to begin

4\. **Wait for installation to complete:**

- Installation may take 30-60 minutes depending on internet speed

- Requires several gigabytes of disk space

5\. **Verify installation:**

- Open Command Prompt or PowerShell

- Type `latex --version` to verify
:::

## Windows Installation Requirements {#windows-installation-requirements .unnumbered}

  **Requirement**        **Details**
  ---------------------- -----------------------------------
  Operating System       Windows 7 or later
  Disk Space             5-7 GB for full installation
  Administrator Rights   Required for installation
  Internet Connection    Required for downloading packages

------------------------------------------------------------------------

# MacTeX - MacOS Variant {#sec:mactex}

    • MacTeX - a variant for MacOS.

## Generated figure (simulation) {#generated-figure-simulation-4 .unnumbered}

MacTeX for MacOS.

## MacTeX Information {#mactex-information .unnumbered}

::: framed
**MacTeX - TeX Live for MacOS:**

MacTeX is the MacOS-specific distribution of TeX Live. It includes:

- Complete TeX Live installation

- Mac-specific tools and utilities

- TeXShop editor

- LaTeXiT equation editor

- BibDesk reference manager

- Easy installer package (.pkg)

**Installation:**

1.  Download MacTeX from `https://tug.org/mactex/`

2.  Open the downloaded .pkg file

3.  Follow the installer instructions

4.  Installation takes approximately 5-7 GB

**Alternative:** BasicTeX (smaller version) for users with limited disk
space.
:::

------------------------------------------------------------------------

# Editor Installation - Visual Studio Code {#sec:vscode}

    For editing LaTeX documents, Visual Studio Code with LaTeX extensions is recommended.

## Generated figure (simulation) {#generated-figure-simulation-5 .unnumbered}

VS Code installation options.

## Screenshot {#screenshot-2 .unnumbered}

::: center
![image](vscode-install-options.png){width="80%"}
:::

## VS Code Installation Guide {#vs-code-installation-guide .unnumbered}

::: framed
**Visual Studio Code Installation:**

1\. **Download VS Code:**

- Visit: `https://code.visualstudio.com/`

- Download the installer for your operating system

2\. **Installation options (important):**

- **Add \"Open with Code\" action** - Recommended for easy file access

- **Add to PATH** - Essential for command line usage

- **Register Code as editor** - Associates .tex files with VS Code

3\. **Recommended LaTeX extensions:**

- LaTeX Workshop

- LaTeX Utilities

- LTeX - LanguageTool grammar checker
:::

------------------------------------------------------------------------

# Verification and First Test {#sec:verification}

    After installation, verify that TeX Live is properly installed by creating a simple document.

## Generated figure (simulation) {#generated-figure-simulation-6 .unnumbered}

Testing the installation.

## Screenshot {#screenshot-3 .unnumbered}

::: center
![image](texlive-test.png){width="80%"}
:::

## Test Document {#test-document .unnumbered}

::: framed
**Create a test file `test.tex`:**

``` {.latex language="TeX"}
\documentclass{article}
\begin{document}
Texlive ok? HAHAHAHAHAHA!!!!!!!! okokok
\end{document}
```

**Compile the document:**

    pdflatex test.tex

**Expected output:**

- `test.pdf` should be created

- No error messages

- PDF viewer should display \"Hello, TeX Live!\"
:::

## Verification Commands {#verification-commands .unnumbered}

  **Command**            **Purpose**
  ---------------------- --------------------------------
  `latex --version`      Show LaTeX version information
  `pdflatex --version`   Show pdfTeX version
  `tex --version`        Show TeX version
  `tlmgr --version`      Show TeX Live Manager version

------------------------------------------------------------------------

# Conclusion: TeX Live Installation Methodology {#conclusion-tex-live-installation-methodology .unnumbered}

After comprehensive analysis of TeX Live installation methods, here is
the structured methodology for successfully installing and configuring
TeX Live:

## 1. Installation Methods Comparison {#installation-methods-comparison .unnumbered}

  **Method**        **Platform**             **Advantages**              **Disadvantages**
  ----------------- ------------------------ --------------------------- -----------------------
  Package Manager   Linux, Windows (Choco)   Easy, integrated            May be outdated
  Manual Install    All platforms            Latest version, control     Complex, manual steps
  MacTeX            MacOS                    Optimized, tools included   MacOS only

## 2. Recommended Installation Workflow {#recommended-installation-workflow .unnumbered}

**Step : Choose installation method based on OS**

- **Linux (Ubuntu/Debian)**: `sudo apt install texlive-full`

- **Linux (others)**: Manual installation or distribution packages

- **Windows**: Manual installer or Chocolatey

- **MacOS**: MacTeX from official website
