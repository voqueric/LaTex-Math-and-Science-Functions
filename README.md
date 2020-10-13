# LaTex-Math-and-Science-Functions

Use the following line within the document preamble to determine if compilation take place in a Linux operating system or Windows operating system:

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
