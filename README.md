# Building a futuristic Lisp operating system

![A modern Lisp machine for the ultimate programming experience](screenshot.png "Screenshot of lisp hacking in exwm running on Guix System")

Through my eponymous nonprofit project [enzu.ru](https://enzu.ru), I am currently working on the [GNU operating system](https://www.gnu.org/) in order to create a [libre](https://www.gnu.org/philosophy/free-sw.html) Lisp-based workstation, built upon the [Guix System](https://guix.gnu.org) GNU/Linux distribution and [exwm window manager](https://github.com/ch11ng/exwm). Pairing these two together creates a programming environment and computing style that can be referred to as "Lisp user space".

If in [POSIX](https://en.wikipedia.org/wiki/POSIX) everything is [truly a file](https://en.wikipedia.org/wiki/Everything_is_a_file), then [the logical conclusion](https://github.com/NetBSD/src/blob/trunk/doc/roadmaps/desktop#L259) is that the ideal POSIX desktop environment should be a file editor, and the only editor that can function as such is [GNU Emacs](https://www.gnu.org/software/emacs/).

Emacs has applications for all the major desktop environment functions, such as [window management](https://github.com/ch11ng/exwm), [file management](https://github.com/sunrise-commander/sunrise-commander), [web browsing](https://github.com/emacsmirror/elpher), [mail](https://notmuchmail.org/notmuch-emacs/), [streaming music](https://github.com/agrif/pianobar.el), [chatting](https://www.gnu.org/software/emacs/manual/html_mono/erc.html), [shell management](https://www.gnu.org/software/emacs/manual/html_mono/eshell.html), [version control](https://magit.vc/), and [life organization](https://orgmode.org/). All these tools can be hacked live with Lisp as you use them.

This computing style provides an [introspective](https://www.gnu.org/software/guile/manual/html_node/Introspection.html), [hackable](https://www.gnu.org/philosophy/rms-hack.en.html), and [transactionable](https://guix.gnu.org/en/blog/2018/multi-dimensional-transactions-and-rollbacks-oh-my/) programming environment that is centered on [text-based user interfaces](https://en.wikipedia.org/wiki/Text-based_user_interface) instead of [graphical user interfaces](https://en.wikipedia.org/wiki/Graphical_user_interface), and that can be used [without a mouse](https://www.nongnu.org/ratpoison/inspiration.html).

This computing style exists to provide advanced hackers with a programming environment more reflective of their ethos and virtuosity. Most operating systems and desktop environments aim to fulfill the needs of the casual non-technical user; this project only aims to provide tools and documentation for advanced free software users who are willing to become fluent in Lisp.

The backend (operating system) is mostly defined in Scheme Lisp and the frontend (desktop environment) and its tools are mostly coded in Emacs Lisp. Both can be hacked live in a REPL, making it a pure expression of the free software ethic, and an incredibly versatile tool for a skilled programmer. I continue to progress on publishing documentation and tools for this rich computing style, a modern iteration of the [Lisp machines](https://en.wikipedia.org/wiki/Lisp_machine) of yore.

Follow me on GitHub to keep track of my contributions to various Lisp user space codebases! Development on the GNU operating system itself is limited to the official mailing lists for each project.

Are you interested in having an advanced Lisp-based workstation that you can hack live to suit your needs? Getting started is easy:

- Install the [Guix System GNU/Linux distribution](https://guix.gnu.org)
- Install Emacs with `guix install emacs`
- Install [Geiser](https://www.nongnu.org/geiser/) and [exwm](https://github.com/ch11ng/exwm) for Emacs (`M-x package-install geiser`, `M-x package-install exwm`)
- [Bootstrap exwm](https://github.com/ch11ng/exwm/wiki#bootstrap) on Emacs instantiation
- Setup your [.xsession](https://github.com/ch11ng/exwm/wiki/Configuration-Example#configuration-of-x-init-script) file so that the login manager can boot into Emacs
