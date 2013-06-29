Copyright (CC BY-NC-SA 3.0 AU) 2013 by T. M. Griffiths under the creative commons licence(attribution, non-comercial, share alike): http://creativecommons.org/licenses/by-nc-sa/3.0/au/ 

This work may be distributed and/or modified under the conditions of the LaTeX Project Public License version 1.3c: http://www.latex-project.org/lppl/lppl-1-3c.txt

This Package redefines the \maketitle command for LaTeX documents and generates
a title page for a UOW thesis. Use this package with the book class to typeset your thesis. 

The UOW default dimensions can be implimented with:
\usepackage{geometry}
    \geometry{a4paper,inner=4.0cm, outer=2cm, top=3cm, bottom=2cm}               
                   
Created by Thomas M. Griffiths (tmg994[at]uowmail[dot]edu[dot]au) 2013-06-17             


------------Basic Usage------------

\usepackage[]{uowthesistitlepage}

\begin{document}
%Standard fields of \maketitle
\title{A Pretty Swish Title} 
\author{Average J. Blow}
    %If you use the hyperref package you can add a mailto link, so that clicking on your name opens an email to you.
	
%The new fields from the \maketitle renewal (see code below).
\degree{That Degree You've Been Studying} 
    %Write it in full: e.g. Bachelor of Science Medicinal Chemistry Advanced Honours
\school{Your School} 
    %e.g Chemistry
\supervisor{supervisor 1, supervisor 2 \& supervisor 3}
    %A list of your supervisors, can be turned off with the nosupervisor package option in the preamble or switched to multiple (more thn one) with the package option multiplesupervisors
    
\maketitle