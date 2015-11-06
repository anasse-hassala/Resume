# moderncv

These are the files of the `moderncv` LaTeX package, with some modifications I've made.

`moderncv` was created by Xavier Danaux and can be downloaded from [CTAN][]. Note that the files in that page are not the same I'm using here, they are updated. I'm using an older version of the package because it let me do some things that the new one's doesn't. For example, using a roman font with the classic theme is not allowed in the new version.

Besides that, I made some tweaks in the code, mainly:

* `\github` and `\linkedin` commands to put your GitHub and Linkedin links together with your other personal information (with logos, see below).
* `\lattes` command, so that Brazilian users can insert their link to "[Currículo Lattes][Lattes]" (with the [CNPq][] logo).
* Keep a sans-serif font for page numbers.

To generate the logos for GitHub and Linkedin, I've used this code from [tex.stackexchange][] (thanks to Paulo Cereda and Gonzalo Medina). I've created `pgf` files, opened them at [Qtikz][], and exported as `pdf` files.

The CNPq logo was downloaded directly from the [CNPq visual identity website][lmarca]. I've just extracted the "head" (!), made it grey, and converted to `pdf` using [Inkscape][] and [Gimp][].

Main files modified were:

* `moderncv.cls` (lines 204, 205, 206, 259, 260, 261, 413)
* `moderncvthemeclassic.sty` (lines 152, 153, 154)

See how it is in this [template][temp-pdf] (source [here][temp-src]). (NOTE for the geeks: the Spock info is just illustrative, no care was taken about real facts and dates! No offence intended. LLAP `\\//`)

## License

The original `moderncv` package is Copyright Xavier Danaux, and distributed under [The LaTeX Project Public License (lppl1.3)][lppl].

Modifications here are under the same license (lppl1.3).


[CTAN]: http://www.ctan.org/tex-archive/macros/latex/contrib/moderncv/
[tex.stackexchange]: http://tex.stackexchange.com/questions/70216/adding-sections-such-as-linkedin-and-github-to-a-moderncv-footer
[Qtikz]: http://www.hackenberger.at/blog/ktikz-editor-for-the-tikz-language/
[temp-pdf]: template_moderncv.pdf
[temp-src]: template_moderncv.tex
[lppl]: http://www.ctan.org/license/lppl1.3
[Lattes]: http://lattes.cnpq.br
[CNPq]: http://cnpq.br
[lmarca]: http://cnpq.br/web/guest/lmarca-cnpq
[Inkscape]: http://inkscape.org
[Gimp]: http://www.gimp.org
