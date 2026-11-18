# GMU Proposal Template

This is a reusable template extracted from the current folder. It does not include the original author’s research content, figures, personal information, or bibliography database.

`gmuETD.sty` is preserved unchanged. `main.tex` retains the original template author attribution and disclaimer.

The formatting style comes from the local files, which include revision records from 2023. The latest GMU submission requirements have not been independently verified.

The proposal cover page has been replaced with an editable placeholder based on the locally customized cover page. It should not be interpreted as an official or university-wide GMU proposal format requirement.

## How to Use

1. Upload the corresponding ZIP file to Overleaf as a new project.
2. Set `main.tex` as the main file and use `pdfLaTeX` as the compiler.
3. Edit `metadata.tex` to update your name, title, department, advisor, committee members, and other information.
4. Write your own content in the `chapters/` directory. To add a new chapter, add the corresponding `\include` command in `main.tex`.
5. `references.bib` is intentionally left empty. After adding your own references and using `\cite{citation-key}`, remove the `%` characters before the `\bibliographystyle` and `\bibliography` lines in `main.tex`.
6. Enable the commented appendix, List of Figures, and List of Tables sections in `main.tex` as needed.
7. Keep one blank Overleaf project as a master template and duplicate it whenever starting a new document.  
   You can download the project source as a ZIP file for backup or later re-import. Downloading the PDF only saves the compiled output.

## File Structure

`main.tex`  
Main file and chapter order

`metadata.tex`  
Personal information and metadata using English placeholders

`gmuETD.sty`  
Original GMU formatting style

`chapters/`  
Placeholder files for main chapters

`references.bib`  
Your own bibliography entries

`appendix.tex`  
Optional appendix

`proposal-cover.tex`  
Editable proposal cover page


Local compilation:

`latexmk -pdf main.tex`
