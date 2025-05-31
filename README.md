# Latex-templete
Style guide for latex  documents and beamer presentations. 

Latex is a highly configurable, composable typesetting engine. 
It can produces nice documents, ppts (presentations). Many people find latex to
be difficult thing to graps. To some extent this true for complete 
beginer but if  we understand few basic structure of latex then 
things become bit easier. 

## Beamer
Beamer is a latex package that allows you to create presentations.
It is similar to PowerPoint, but it uses LaTeX for typesetting.
(See [Beamer User Guide](https://ctan.org/pkg/beamer?lang=en) for more information.)


#### Style Guide 
- Use `columns` environment to create columns in your slides.
    ```latex
        \begin{columns}
            \begin{column}{0.5\textwidth}
                % Left column content
            \end{column}
            \begin{column}{0.5\textwidth}
                % Right column content
            \end{column}
        \end{columns}
    ```
- Use `itemize` or `enumerate` environments for lists.
    ```latex
        \begin{itemize}
            \item First item
            \item Second item
        \end{itemize}
    ```
- Use `block, alertblock, exampleblock` for highlighting important information.
    ```latex
        \begin{block}{Block Title}
            Block content goes here.
        \end{block}
    ```
- use `includegraphics` to add images.
    ```latex
        \includegraphics[width=\textwidth]{image.png}
    ```
- use `tcolorbox` for colored boxes.
    ```latex
        \begin{tcolorbox}[colback=blue!5!white,colframe=blue!75!black]
            Tcolorbox content goes here.
        \end{tcolorbox}
    ```
- Use `checkboxes` and `xbox` for tasks or items.
	```latex		
	\begin{exampleblock}{Classical Model}
		\begin{itemize}
			\item $\CheckedBox$ Can explain bound state.
			\item $\CheckedBox$ Can explain spin-polarized STM
			\item $\XBox$ Kondo (quantum) effects ignored.
			\item $\XBox$ Internal degrees (spin, ..) are is ignored.
		\end{itemize}
	\end{exampleblock}
    ```		
- Add footnote using `footnote` command.
    ```latex
        This is a footnote\footnote{This is the footnote text.}.
    ```
- Use `hyperref` package for clickable links.
    ```latex
        \usepackage{hyperref}
        \href{https://example.com}{Click here}
    ```
- Add a thanks to end of slide 
    ```latex             
        \begin{frame}[plain]
            \begin{center}
                {\fontsize{50}{60}\selectfont \textbf{Thank You.}}
            \end{center}
        \end{frame}
    ```    


