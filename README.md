# Building a futuristic Lisp operating system

![A modern Lisp machine for the ultimate programming experience](screenshot.png "Screenshot of lisp hacking in exwm running on Guix System")

Through my eponymous nonprofit [enzu.ru](https://enzu.ru), I am currently working on the [GNU operating system](https://www.gnu.org/) in order to create a [libre](https://www.gnu.org/philosophy/free-sw.html) Lisp-based workstation, tied together by the [Guix System](https://guix.gnu.org) GNU/Linux distribution.

My personal goal is to build an [introspective](https://www.gnu.org/software/guile/manual/html_node/Introspection.html), [hackable](https://www.gnu.org/philosophy/rms-hack.en.html), and [transactionable](https://guix.gnu.org/en/blog/2018/multi-dimensional-transactions-and-rollbacks-oh-my/) programming environment that is centered on [text-based user interfaces](https://en.wikipedia.org/wiki/Text-based_user_interface) instead of [graphical user interfaces](https://en.wikipedia.org/wiki/Graphical_user_interface).

The backend (operating system) is mostly defined in Scheme Lisp and the frontend (desktop environment) and its tools are mostly defined in Emacs Lisp. For portability, I write most of my personal tools in Common Lisp.

Follow me on GitHub to keep track of my contributions to various Lisp userspace codebases! Development on the GNU operating system itself is limited to the official mailing lists for each project.

Are you interested in having a Lisp-based workstation? I keep my configuration and code public as a learning tool! Getting started is easy:

- Install the [Guix System GNU/Linux distribution](https://guix.gnu.org)
- Modify my [Scheme code](https://github.com/enzuru/guix-profiles) and run them to setup your own user
- Log into the user and you will be booted into the [exwm window manager](https://github.com/ch11ng/exwm)
