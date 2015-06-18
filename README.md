# F3LaTeX Plugin#

## Summary ##

F3LaTeX (F3LP) is a plugin for [Gajim][1], based upon [Latex-Plugin][2] (LP) by Yves Fischer and Yann Leboulanger.

As LP is quite limited, I decided to write my own plugin allowing not only math formula, but common document contents with a focus on modern standards for math typesetting.

## Differences to Latex-Plugin ##

* Uses modern techniques: KOMA, AMS, mathtools, lmodern,…
* Not restricted to math formulas: Your text gets inserted right behind `\begin{document}`, you may even decide which math. environement you want to choose.
* Uses pdflatex and convert instead of latex and dvipng, thus it is possible to use ps-sequences (i.e. for tikz)
* Might work with LP still enabled (uses `%% %%` to delimit code)

## Caution! ##

Original LP restricts the usage of many LaTeX-Macros such as `\renewcommand`. Allowing them in F3LP gives much more possibilities, but may be a security risk. Usage at your own risk!

## Install ##

Move the f3latex-folder to your local gajim-plugin-folder (usually something like `~/.gajim/plugins/` or `~/.local/share/gajim/plugins/`, then activate it using the Plugin-Manager.

[1]: http://gajim.org/ "Gajim"
[2]: https://trac-plugins.gajim.org/wiki/LatexPlugin "Latex Plugin"
