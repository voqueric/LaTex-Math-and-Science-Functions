# LaTex-Math-and-Science-Functions
1. Place files into the final destination directory on your system.
2. Open 00--Science_and_Math.tex
3. Locate these two lines, and change the folder in each to the final destination directory for each operating system:

```
\newcommand{ \mylinuxlatexmathpath }[0]{/linux/path/to/file}
\newcommand{ \mywinlatexmathpath }[0]{C:/windows/path/to/file}
```
4. Close and save file.
5. Add the following line within the document preamble to determine if compilation takes place within a Linux operating system or Windows operating system:

```
\documentclass[letterpaper,10pt]{article}

% Place this line in the preamble section
\InputIfFileExists{/linux/path/to/file/00--Science_and_Math.tex}%
  {}%
  {\input{C:/windows/path/to/file/00--Science_and_Math.tex}}
  
\begin{document}

% Some stuff here.

\end{document}
```
This file automatically loads the other files in this repository.  Each file contains command descriptions and arguments to guide use.  I will do my best to not change command names and arguments to maintain backwards compatibility as much as possible.
