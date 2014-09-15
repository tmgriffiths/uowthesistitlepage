## This is the README for uowthesistitlepage.sty Version 2.0, 2014-01-07

### ABOUT
This Package redefines the `\maketitle` command for LaTeX documents and generates a title page for a UOW thesis in accordance with the uow branding guidelines. Use this package with the book class to typeset your thesis (it will work with report though if you do so desire). The package also provides the `\declaration` command. This typesets the declaration (see below) that your thesis/dissertation/report is your own work, required in the front of each PhD Thesis.

The `uowthesistitlepage.sty` style file **is not** a complete thesis template or document class, it only typesets the title page (honours thesis by default) and declaration. The directory `thesis_template` contains a template thesis document that can be used as a basis for your document.

### Required Packages
- setspace
- etoolbox
- graphicx 
- geometry


###BASIC USAGE
```latex
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
```
   
## For the Inquisitive, Some of the Output
### Wording of the Declaration (example option `phd`)

**Declaration**

*I, <Student’s Full Name>, declare that this thesis submitted in fulfilment of the requirements for the conferral of the degree Doctor of Philosophy, from the University of Wollongong, is wholly my own work unless otherwise referenced or acknowledged. This document has not been submitted for qualifications at any other academic institution.*



----------------------------

<Student’s Full Name>
January 9, 2014




### Default Margins for UOW Theses.

The UOW default dimensions (as done by the style file) can be implemented with:

```latex
   \usepackage{geometry}
   \geometry{a4paper,inner=4.0cm, outer=2cm, top=3cm, bottom=2cm}               
```
                
Created by Thomas M. Griffiths (tmg994[at]uowmail[dot]edu[dot]au) 2014-09-15

## LEGAL
Copyright (CC BY-NC-SA 3.0 AU) 2014 by T. M. Griffiths under the creative commons licence(attribution, non-comercial, share alike): http://creativecommons.org/licenses/by-nc-sa/3.0/au/. This work may be distributed and/or modified under the conditions of the LaTeX Project Public License version 1.3c: http://www.latex-project.org/lppl/lppl-1-3c.txt
