# Talks
## Basic design
The simple template and examples is in master.
Each talk is in a branch with a name starting with year and month (YYYY_MM).
Each branch have a commont sty file and example file but a unique LaTeX file

After clone the repo, to switch to an specific branch use (e.g BRANCH=2019_SARAH)
```bash
git checkout -B BRANCH # without origin_etc prefix
git pull origin BRANCH
```


* Install `texlive-fonts-extra`
* Install [mtheme](https://github.com/matze/mtheme)
* Install the fonts: mtheme/docker/getFiraFont.sh



Run as
```bash
xelatex master.tex
```

<!-- figures/master.svg -->
[![Image inheritance diagram](http://interactive.blockdiag.com/image?compression=deflate&encoding=base64&src=eJxNjs0KgzAQhO8-RfDupdCTWOhzlCJrsmpokpW4Qmnpu9eNv6fMfjOzm8aRfhkLnfpmSlG0GBjYUlCVGihyBMvl7BhsYXJctxR4tB-c7avwu3o4aNBVuYeRMebPMku4uKmGOmIot3FkCAaiKTwZdDuFCL1klvTRqzX5HofDWoEkGN8wipPEqeNJw6khY8pbnhzE1Fik0GXfRegqhc6v7q1DwZveb6Zw-vKxoMx-f4I3Z3A)](http://interactive.blockdiag.com/?compression=deflate&src=eJxNjs0KgzAQhO8-RfDupdCTWOhzlCJrsmpokpW4Qmnpu9eNv6fMfjOzm8aRfhkLnfpmSlG0GBjYUlCVGihyBMvl7BhsYXJctxR4tB-c7avwu3o4aNBVuYeRMebPMku4uKmGOmIot3FkCAaiKTwZdDuFCL1klvTRqzX5HofDWoEkGN8wipPEqeNJw6khY8pbnhzE1Fik0GXfRegqhc6v7q1DwZveb6Zw-vKxoMx-f4I3Z3A)


# Official Metroplis README starts here
## Metropolis
Really installled as a git repo in:
/usr/share/texlive/texmf-dist/tex/latex/mtheme
Go there to pull and
make sty


**NOTICE: The package name changed from *m* to *metropolis*!**

Metropolis is a simple, modern Beamer theme suitable for anyone to use. It tries
to minimize noise and maximize space for content; the only visual flourish it
offers is an (optional) progress bar added to each slide. The core design
principles of the theme were described in a blog post
[here](http://bloerg.net/2014/09/20/a-modern-beamer-theme.html).

Not convinced? Have a look at the [demo slides](demo/demo.pdf).

![Sample](http://i.imgur.com/Bxu52fz.png)


## Installation

Installing Metropolis, like any Beamer theme, involves four easy steps:

1. **Download the source** with a `git clone` of the [Metropolis repository](https://github.com/matze/mtheme) or as a [zip archive](https://github.com/matze/mtheme/archive/master.zip) of the latest development version.

2. **Compile the style files** by running `make sty` inside the downloaded
    directory. (Or run LaTeX directly on `source/metropolistheme.ins`.)

3. **Move the resulting `*.sty` files** to the folder containing your presentation. To use Metropolis with many presentations, run `make install` or move the `*.sty` files to a folder in your TeX path instead (might require `sudo` rights).

4. **Use the theme for your presentation** by declaring `\usetheme{metropolis}` in
    the preamble of your Beamer document.


## Usage

The following code shows a minimal example of a Beamer presentation using
Metropolis.

```latex
\documentclass{beamer}
\usetheme{metropolis}           % Use metropolis theme
\title{A minimal example}
\date{\today}
\author{Matthias Vogelgesang}
\institute{Centre for Modern Beamer Themes}
\begin{document}
  \maketitle
  \section{First Section}
  \begin{frame}{First Frame}
    Hello, world!
  \end{frame}
\end{document}
```

Detailed information on using Metropolis can be found in the [manual (PDF)](doc/metropolistheme.pdf).


## License

The theme itself is licensed under a [Creative Commons Attribution-ShareAlike
4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/). This
means that if you change the theme and re-distribute it, you *must* retain the
copyright notice header and license it under the same CC-BY-SA license. This
does not affect the presentation that you create with the theme.
