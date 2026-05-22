# IMC Problem Booklet

LaTeX document that assembles IMC problems using LuaLaTeX.

- Build: `latexmk -g -lualatex -interaction=nonstopmode -halt-on-error imc-booklet.tex`
- Structure: `problems/<year>/<problem>/problem_en.tex` (driver uses folder names for numbering)
- Language: set `\IMCLanguage` in `imc-booklet.tex` (default `en`)
- Notes: `imc-booklet.tex` uses Lua (lfs) to collect and \input{} problem files. Edit that file to change formatting.

Contributions: add new problem folders under `problems/` following the existing structure.