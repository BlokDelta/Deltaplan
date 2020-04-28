# Deltaplan

Source files for the Deltaplan (Dutch version of a Green New Deal), as proposed by the [Delta group.](https://blokdelta.nl/)

# Development

### Clone repo

	git clone https://github.com/BlokDelta/Deltaplan.git

### Render pdf

We use the XeLaTeX engine. This is defined with the `!TEX program` statement in `main.tex` and most editors should pick up on this automatically. To render the file manually, use e.g.

	latexmk -pdf -xelatex

When using BasicTeX, you might need to install additional packages:

	sudo tlmgr install xargs biblatex biblatex-apa biber todonotes csquotes

Possibly at some point also

	sudo tlmgr install footmisc enumitem tocbibind logreq cleveref titlesec multicol


You also need to have Work Sans installed. Download it [here](https://weiweihuanghuang.github.io/Work-Sans/) or use Homebrew:

	brew cask install font-work-sans
