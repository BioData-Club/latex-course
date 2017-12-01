OHSU BioData Club:  LaTex and Collaborative Writing Software Introduction
============
The slides for this workshop and their LaTeX source
code were forked from [this github repository](https://github.com/jdleesmiller/latex-course) under a permissive MIT license.

The aim of this session is to get you attuned to the basics of writing in LaTeX as quickly as possible. The material is presented as a set of examples.  Broader concepts and techniques are explained as they arise. Each part includes exercises that can be completed on [Overleaf](https://www.overleaf.com), a free online LaTeX editor, so **you don't have to worry about getting LaTeX and related tools installed on your computers.**

We've yet to customize these slides for BioData Club, as they already do the job of introducing learners to LaTeX quite well. There is enough material in these slides for multiple workshops, but we'll at least aim to get through **The Basics**, and hopefully some of part 2 on Structured Documents.  If you're already familiar with writing in LaTex, you should skip forward - also we'll have advanced users on hand to brainstorm and answer questions. 

In our session, we'll access the the slides from [here](https://www.overleaf.com/latex/learn/free-online-introduction-to-latex-part-1#.WiHWDrQ-eqA)

Links to indvidual lesson files are below.

1. [The Basics](http://jdleesmiller.github.io/latex-course/en/part1.pdf): ideas, syntax, equations, environments, packages

1. [Structed Documents &
More](http://jdleesmiller.github.io/latex-course/en/part2.pdf): titles, sections, cross-references, figures, tables, bibliographies.

1. [Not Just Papers: Presentations & More](http://jdleesmiller.github.io/latex-course/en/part3.pdf): recap exercise, presentations with beamer, drawings with
tikz.

Feel free to use however you like --- contributions welcome!

Further Slide Development...for down the road
-----------

You may need to install some extra LaTeX packages and system packages in order
to build the slides yourself.

1. The [minted package](http://www.ctan.org/pkg/minted) provides syntax
highlighting. It is installed by default in recent versions of TeX Live.

1. The minted package calls out to the
[pygments syntax highlighter](http://pygments.org/), which is written in python.
The relevant package is python-pygments in Debian / Ubuntu
(`sudo apt-get install python-pygments`).

1. There is a simple `Makefile` that manages the build. To use it, you'll
probably need to be on Linux, and you will need `make`.

The slides include links to exercises that open in Overleaf. The exercise
source files are hosted on github. If you want to use exercise files in another
location, you can [fork](https://help.github.com/articles/fork-a-repo) this
github repository and then change the `\fileuri` macro in `preamble.tex`:
```
\newcommand{\fileuri}{https://raw.github.com/jdleesmiller/latex-course/master/en}
```
so that instead of pointing to `jdleesmiller/latex-course`, it points to
`your-github-user-name/latex-course`. Then, once you've pushed your changed
exercise files to github, the slides will load them up in Overleaf.

The `deploy-to-gh-pages.sh` script builds the slides using the Makefile and
copies the slides over to the `gh-pages` branch, which is available at
`https://jdlm.info/latex-course` thanks to
[github pages](http://pages.github.com/).

License
-------

The slides and source are released under the MIT license. See the LICENSE file.

Original Credits
-------

* Diana A -- found that exercise links had broken
* Sana A -- pointed out an error in part 1
* Andy Roberts -- the chick(en) image is from [one of his articles](http://www.andy-roberts.net/writing/latex/importing_images)
* Ruby Trinh -- for organising the original short courses
