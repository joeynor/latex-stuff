# latex-stuff

This is just some personal notes for me to lookup to do some things on latex. 


## Bibliography stuff

### There are situations I need to list my publications, and somehow sort it and arrange it by the type of publications. 
The following latex code helps in doing this. 
```
\documentclass{article}
\usepackage[backend=biber, style=numeric, sorting=ydnt]{biblatex}

\addbibresource{papers.bib}

\begin{document}
H-Index: 9
Citations: 300
\nocite{*}

\printbibliography[title={Articles and Journals}, type=article]

\printbibliography[title={Conference Proceedings}, type=inproceedings]

\printbibliography[title={Books}, type=book]
\printbibliography[title={Others}, type=incollection]
\end{document}
```

You can change the style from numeric to authoryear to get rid of the numbers.


