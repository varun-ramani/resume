# Resume
This is the source code for my resume, using a template sourced from CareerCup.

## Instructions for Arch
### TeXLive Setup
- Install TeXLive by running `yay -S texlive`
- Proceed to install Calibri with `yay -S ttf-ms-win10-auto`
### Compilation


## Compilation
- To set up LaTeX on macOS, run `brew install --cask basictex` to obtain a basic LaTeX environment.
- Once `tlmgr` is available, run `sudo tlmgr install texliveonfly` to install software that 
  automatically sources all the necessary packages.
- Find and install the Calibri font.
- In the project root, run `texliveonfly --compiler=lualatex resume.tex` to automatically install necessary packages and generate
  an initial compilation of this project.

## VSCode Setup
- Run `sudo tlmgr install latexmk`.
- Install LaTeX Workshop in VSCode to get LaTeX functionality enabled.
- Enable LuaLaTeX as the compiler in LaTeX workshop.
