# LaTex-Math-and-Science-Functions

Use the following line within the document preamble to determine if compilation take place in a Linux operating system or Windows operating system:

'''
\InputIfFileExists{/linux/path/to/file/00--Science_and_Math.tex}%
  {}%
  {\input{C:/windows/path/to/file/00--Science_and_Math.tex}}
'''
This file automatically loads the other files in this repository.  Each file contains command descriptions and arguments to guide use.
