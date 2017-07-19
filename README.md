This is the README for uowthesistitlepage.sty Version 3.0, 2017-07-18
=====================================================================

About
-----

This Package redefines the `\maketitle` command for LaTeX documents and generates a title page for a UOW thesis in accordance with the uow branding guidelines. Use this package with the book class to typeset your thesis (it will work with report though if you do so desire). A copyright declaration is printed on the page immediately following the title page, including the required acknowledgement of the Australian Government Research Training Program Scholarship. The package also provides the `\declaration` command. This typesets the declaration (see below) that your thesis/dissertation/report is your own work, required in the front of each PhD Thesis.

This package *is not* a complete thesis template or document class, it *only* typesets the title page and declaration. This package is designed to do as little to your document as possible. It won't set the margins, spacing, or typeface used in your document. This version is a major redesign of the title page to coincide the re-branding of UOW during 2016. It also adds the copyright statement and acknowledgement of the Australian Government Research Training Partnership Scholarships. Be sure to use the new version of the UOW crest (below). A copy is distributed with the uow thesis template on UOW website. It follows the UOW thesis guidelines and is has a basic setup ready to get you started with your thesis. For those starting off on their own, the following code will give you a document that satisfies the UOW thesis guidelines.

````latex
\documentclass[twoside,12pt,a4paper]{book}
\usepackage{geometry}
  \geometry{a4paper,inner=4.0cm, outer=2cm, top=3cm, bottom=2cm}

\usepackage{setspace}
\onehalfspacing
% or
% \doublespacing

% to use in Times New Roman instead of the LaTeX default, latin modern.
\usepackage{mathptmx}
````


Required Packages
-----------------

- setspace
- etoolbox
- graphicx
- geometry

Basic Usage
-----------

````latex
   \usepackage[]{uowthesistitlepage}`

   % Standard fields of \maketitle
      \title{A Pretty Swish Title}
      \author{Average J. Blow}
      \date{Month Year}

   % The new fields from the \maketitle renewal (see code below).
      \degree{That Degree You've Been Studying} 
         % Write in full: e.g. Bachelor of Science Honours
      \school{Your School}  
         % e.g Chemistry
      \supervisor[x]{Supervisor 1, Supervisor 2,... \& Supervisor x}
         % A list of your supervisors, can be turned off with the 
         % nosupervisor package option in the preamble or switched 
         % to multiple (more than one) with the package option 
         % multiplesupervisors
    
   % And the optional field
      \cosupervisor[number of co-supervisors]{Co-supervisors 1, Co-supervisor 2,... \& Co-supervisor x}

   \begin{document}
       
   \maketitle
   
   \declaration 
   
   % Your Thesis...
   
   \end{document}
````

Wording of the Declaration (example option 'phd')
-------------------------------------------------

> **Declaration**
>
> I, *Student’s Full Name*, declare that this thesis submitted in fulfilment of the requirements for the conferral of the degree *Doctor of Philosophy*, from the University of Wollongong, is wholly my own work unless otherwise referenced or acknowledged. This document has not been submitted for qualifications at any other academic institution.
>
>
>
> Student’s Full Name 
>
> January 9, 2014
>


Default Margins for UOW Theses
------------------------------

The UOW default dimensions (as done by the style file) can be implemented with:

````latex
   \usepackage{geometry}
   \geometry{a4paper,inner=4.0cm, outer=2cm, top=3cm, bottom=2cm}
````

Created by Thomas M. Griffiths (tmg994[at]uowmail[dot]edu[dot]au) 2017-07-19

Legal
-----

Copyright (CC BY-NC-SA 3.0 AU) 2017 by T. M. Griffiths under the creative commons licence(attribution, non-comercial, share alike): http://creativecommons.org/licenses/by-nc-sa/3.0/au/. This work may be distributed and/or modified under the conditions of the LaTeX Project Public License version 1.3c: http://www.latex-project.org/lppl/lppl-1-3c.txt

