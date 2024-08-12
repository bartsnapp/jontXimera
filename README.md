# Notes:

Ximera does not allow labels to be inside of headings. 

Solution: Move them just below headings



# Title/preamble
Replace
%Chapter 2

%Format for subsection:
\chapter  %[Stream 1: Number Systems ]
	{Stream 1: Number Systems \label{Chap:NS} \label{Sect:NS}}
\index{stream 1}
\setcounter{exercise}{0}

with 
\documentclass{ximera}

\input{preamble.tex}

%Chapter 2

%Format for subsection:
\title  %[Stream 1: Number Systems ]
	{Stream 1: Number Systems}
%\setcounter{exercise}{0} 

\begin{document}
\begin{abstract}
\end{abstract}
\maketitle
\label{Chap:NS} \label{Sect:NS}
\index{stream 1}


be sure add 

\end{document}


# EPS to PDF