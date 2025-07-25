# Building a futuristic Lisp workstation

![GNU/Linux with a Lisp user space on top](screenshot.png "Screenshot of lisp hacking in exwm running on Guix System")

I am currently working on the [GNU operating system](https://www.gnu.org/) in order to create a futuristic Lisp workstation, with Linux as its kernel, and a rich Lisp user space on top.

Some projects that I contribute to (or plan to):

- [GNU/Linux Guix distribution](https://guix.gnu.org)
- [GNU Emacs](https://www.gnu.org/software/emacs/)
- [StumpWM](https://github.com/stumpwm/stumpwm)

Using org-roam-ui, you can [visually navigate](https://enzuru.github.io/lisp-user-space/) how these projects work together to build a Lisp workstation.

Most of my [user space tools are written in Emacs Lisp](https://github.com/enzuru/.emacs.d), with [my window management handled by Common Lisp](https://github.com/enzuru/home), and [my system configuration declaratively written in Guile](https://github.com/enzuru/profiles).

## Features

### High-performance parallel computing

By combining GNU Guix's [high-performance computing emphasis](https://hpc.guix.info/) with [advanced Clojure parallel computing libraries](https://dragan.rocks/software/), one ends up with a powerful workstation for expressing complex workloads in elegant forms.

### Trustless full-source bootstrap

Secure yourself against malevolent state actors and never trust someone else's unverified binaries again, as you can [build from the source all the way down](https://guix.gnu.org/blog/2023/the-full-source-bootstrap-building-from-source-all-the-way-down/).

### Hack your operating system live

Lisp user space provides an [introspective](https://www.gnu.org/software/guile/manual/html_node/Introspection.html), [hackable](https://www.gnu.org/philosophy/rms-hack.en.html), and [transactionable](https://guix.gnu.org/en/blog/2018/multi-dimensional-transactions-and-rollbacks-oh-my/) operating system that can be modified live in a [REPL](https://en.wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop).

### Text-based and keyboard-driven

Lisp user space is centered on [text-based user interfaces](https://en.wikipedia.org/wiki/Text-based_user_interface) instead of [graphical user interfaces](https://en.wikipedia.org/wiki/Graphical_user_interface), and can be used [without a mouse](https://www.nongnu.org/ratpoison/inspiration.html), which makes it easier to use for people living with disabilities as well as power users.

Emacs has text-based keyboard-driven applications for all the major desktop environment functions, such as [window management](https://github.com/ch11ng/exwm), [file management](https://github.com/suntsov/efar), [web browsing](https://github.com/emacsmirror/elpher), [mail](https://notmuchmail.org/notmuch-emacs/), [streaming music](https://github.com/agrif/pianobar.el), [chatting](https://www.gnu.org/software/emacs/manual/html_mono/erc.html), [shell management](https://www.gnu.org/software/emacs/manual/html_mono/eshell.html), [version control](https://magit.vc/), and [life organization](https://orgmode.org/). All these tools can be modified and adjusted live as you use them.

### Perfect complement to POSIX

If in [POSIX](https://en.wikipedia.org/wiki/POSIX) everything is [truly a file](https://en.wikipedia.org/wiki/Everything_is_a_file), then [the logical conclusion](https://github.com/NetBSD/src/blob/cfd6b2f509474ce4eee8adcb3259acbdd754f5e1/doc/roadmaps/desktop#L259) is that the ideal POSIX "desktop environment" should be a file editor, and the only editor that can function as such is GNU Emacs.

### Respects your freedom

The operating system is mostly defined [declaratively](https://en.wikipedia.org/wiki/Declarative_programming) in Scheme Lisp and the applications are mostly coded [imperatively](https://en.wikipedia.org/wiki/Imperative_programming) in Emacs Lisp. Both can be inspected and hacked live in a REPL, making it a pure expression of the libre software ethic, and an incredibly versatile tool for a skilled programmer.

## Follow me!

I continue to progress on publishing tools and documentation for this rich computing style.

[Follow me on GitHub](https://github.com/enzuru) to keep track of my contributions to various Lisp user space codebases! Development on the GNU operating system itself is limited to the official mailing lists for each project. And [follow me on Medium](https://enzuru.medium.com/) in order to follow my latest announcements and tutorials.

## Using Lisp user space

It's remarkably easy to get a Lisp user space setup on top of Linux:

- Install the [Guix GNU/Linux distribution](https://guix.gnu.org)
- Only install [nonguix](https://gitlab.com/nonguix/nonguix) if you truly require additional hardware support
- Install Emacs (`guix install emacs`)
- Install [Geiser](https://www.nongnu.org/geiser/) (`M-x package-install geiser-guile`) and [SLY](https://github.com/joaotavora/sly) (`M-x package-install sly`)
- Install a Lisp window manager like [exwm](https://github.com/emacs-exwm/exwm) (`M-x package-install exwm`) or [StumpWM](https://github.com/stumpwm/stumpwm) (`guix install stumpwm`)
- Bootstrap your window manager ([exwm](https://github.com/ch11ng/exwm/wiki#bootstrap), [StumpWM](https://github.com/stumpwm/stumpwm/wiki/StartUp))
- Boot into your window manager ([exwm](https://github.com/ch11ng/exwm/wiki/Configuration-Example#configuration-of-x-init-script), [StumpWM](https://stumpwm.github.io/git/stumpwm-git_1.html))
