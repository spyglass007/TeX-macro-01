# TeX-macro-01
TeX-macro-01

%\ProvidesPackage{carlos}[2004/03/24 v1.2 LaTeX package carlos]
%\NeedsTeXFormat{LaTeX2e}


\makeatletter
\catcode`\"=\active
% \def"/{-\nolinebreak\hspace{0pt}} % \nobreakdash-\hspace{0pt}

\newcommand"{\@ifnextchar~ {\@nobreak}%
%                 {\@ifnextchar/ {\@@nobreak}%
                    {\@ifnextchar* {\@@@nobreak}{{\textquotedbl}\hspace{0pt}}}}% }

\def\@nobreak~{-\nolinebreak\hspace{0pt}}
\def\@@nobreak/{\nobreakdash-\hspace{0pt}}
\def\@@@nobreak*{\mbox{-}}
% \def\@error@{Error!}

%\defineshorthand[ngerman]{"/}{\mbox{-}\bbl@allowhyphens}
\makeatother

\catcode`\¨=\active
\def ¨{\'{a}}

\catcode`\·=\active
\def ·{\'{A}}

\catcode`\¸=\active
\def ¸{\'{e}}

\catcode`\¬=\active
\def ¬{\'{E}}

\catcode`\ª=\active
\def ª{\'{\i}}

\catcode`\¹=\active
\def ¹{\'{I}}

\catcode`\¢=\active
\def ¢{\~{n}}

\catcode`\°=\active
\def °{\~{N}}

\catcode`\º=\active
\def º{\'{o}}

\catcode`\¤=\active
\def ¤{\'{O}}

\catcode`\¯=\active
\def ¯{\'{u}}

\catcode`\´=\active
\def ´{\'{U}}

\catcode`\¿=\active
\def ¿{\"{u}}

\catcode`\¡=\active
\def ¡{\"{U}}
