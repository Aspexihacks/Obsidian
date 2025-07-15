```tikz
\usepackage{tikz}
\usepackage[margin=1in]{geometry}
\usetikzlibrary{shapes.geometric}

\begin{document}

\begin{center}
\begin{tikzpicture}

% Outer: Topological spaces
\draw[thick, fill=blue!10] (0,0) ellipse (6 and 3.5);
\node at (0,3.1) {\textbf{Topological Spaces}};

% Metric spaces
\draw[thick, fill=green!10] (0,0) ellipse (4.5 and 2.7);
\node at (0,2.3) {\textbf{Metric Spaces}};

% Normed vector spaces
\draw[thick, fill=yellow!10] (0,0) ellipse (3.3 and 1.9);
\node at (0,1.5) {\textbf{Normed  Spaces}};

% Inner product spaces
\draw[thick, fill=red!10] (0,0) ellipse (2 and 1.1);
\node at (0,0) {\textbf{Inner-Product Spaces}};

\end{tikzpicture}
\end{center}

\end{document}
```
