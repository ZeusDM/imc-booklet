# IMC Problem Booklet

LaTeX document that assembles IMC problems using LuaLaTeX.

- Build English: `latexmk -g -lualatex -interaction=nonstopmode -halt-on-error imc-booklet-en.tex`
- Build Portuguese: `latexmk -g -lualatex -interaction=nonstopmode -halt-on-error imc-booklet-pt.tex`
- Structure: `problems/<year>/<problem>/problem_en.tex` (driver uses folder names for numbering)
- Shared setup: `preamble.tex`
- Compatibility: `imc-booklet.tex` forwards to `imc-booklet-en.tex`
- Notes: the booklet driver uses Lua (lfs) to collect and \input{} problem files. Edit `preamble.tex` to change formatting.

Contributions: add new problem folders under `problems/` following the existing structure.