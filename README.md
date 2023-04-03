# Building a futuristic Lisp workstation

![A modern Lisp machine for the ultimate programming experience](screenshot.png "Screenshot of lisp hacking in exwm running on Guix System")

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=enzuru)](https://github.com/anuraghazra/github-readme-stats)

Through my eponymous nonprofit project [enzu.ru](https://enzu.ru), I am currently working on the [GNU operating system](https://www.gnu.org/) in order to create a [libre](https://www.gnu.org/philosophy/free-sw.html) Lisp workstation, built by pairing the [GNU/Linux Guix distribution](https://guix.gnu.org) with the [exwm window manager](https://github.com/ch11ng/exwm).

Pairing these two together creates a computing style and programming environment that can be referred to as **Lisp user space**. This is a modern iteration of the [Lisp machines](https://en.wikipedia.org/wiki/Lisp_machine) of yore.

### Hack your operating system live

Lisp user space provides an [introspective](https://www.gnu.org/software/guile/manual/html_node/Introspection.html), [hackable](https://www.gnu.org/philosophy/rms-hack.en.html), and [transactionable](https://guix.gnu.org/en/blog/2018/multi-dimensional-transactions-and-rollbacks-oh-my/) programming environment that can be modified live in a [REPL](https://en.wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop).

### Text-based and keyboard-driven

Lisp user space is centered on [text-based user interfaces](https://en.wikipedia.org/wiki/Text-based_user_interface) instead of [graphical user interfaces](https://en.wikipedia.org/wiki/Graphical_user_interface), and can be used [without a mouse](https://www.nongnu.org/ratpoison/inspiration.html).

Emacs has text-based keyboard-driven applications for all the major desktop environment functions, such as [window management](https://github.com/ch11ng/exwm), [file management](https://github.com/suntsov/efar), [web browsing](https://github.com/emacsmirror/elpher), [mail](https://notmuchmail.org/notmuch-emacs/), [streaming music](https://github.com/agrif/pianobar.el), [chatting](https://www.gnu.org/software/emacs/manual/html_mono/erc.html), [shell management](https://www.gnu.org/software/emacs/manual/html_mono/eshell.html), [version control](https://magit.vc/), and [life organization](https://orgmode.org/). All these tools can be modified and adjusted live as you use them.
 
### Perfect complement to POSIX

If in [POSIX](https://en.wikipedia.org/wiki/POSIX) everything is [truly a file](https://en.wikipedia.org/wiki/Everything_is_a_file), then [the logical conclusion](https://github.com/NetBSD/src/blob/trunk/doc/roadmaps/desktop#L259) is that the ideal POSIX "desktop environment" should be a file editor, and the only editor that can function as such is [GNU Emacs](https://www.gnu.org/software/emacs/).

### Respects your freedom

The operating system is mostly defined [declaratively](https://en.wikipedia.org/wiki/Declarative_programming) in Scheme Lisp and the desktop environment and its tools are mostly coded [imperatively](https://en.wikipedia.org/wiki/Imperative_programming) in Emacs Lisp. Both can be inspected and hacked live in a REPL, making it a pure expression of the libre software ethic, and an incredibly versatile tool for a skilled programmer.

### Follow me!

I continue to progress on publishing documentation and tools for this rich computing style.

Follow me on GitHub to keep track of my contributions to various Lisp user space codebases! Development on the GNU operating system itself is limited to the official mailing lists for each project.

### Get Lisp user space running tonight

Are you interested in having an advanced Lisp-based workstation that you can hack live to suit your needs? Getting started is easy:

- Install the [Guix GNU/Linux distribution](https://guix.gnu.org)
- Install Emacs (`guix install emacs`)
- Install [Geiser](https://www.nongnu.org/geiser/) and [exwm](https://github.com/ch11ng/exwm) for Emacs (`M-x package-install geiser-guile`, `M-x package-install exwm`)
- [Bootstrap exwm](https://github.com/ch11ng/exwm/wiki#bootstrap) on Emacs instantiation
- Setup your [.xsession](https://github.com/ch11ng/exwm/wiki/Configuration-Example#configuration-of-x-init-script) file so that the login manager can boot into Emacs
