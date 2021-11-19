# Building a futuristic Lisp operating system

I am currently working on the [GNU operating system](https://www.gnu.org/) in order to create a [libre](https://www.gnu.org/philosophy/free-sw.html) Lisp-based workstation, tied together by the [Guix System](https://guix.gnu.org) GNU/Linux distribution. The backend (operating system) is mostly defined in Scheme Lisp and the frontend (desktop environment) and its tools are mostly defined in Emacs Lisp. For portability, I write most of my personal tools in Common Lisp.

Follow me on GitHub to keep track of my contributions to various Lisp userspace codebases! Development on the GNU operating system itself is limited to the official mailing lists for each project.

Are you interested in having a Lisp-based workstation? I keep my configuration and code public as a learning tool! Getting started is easy:

- Install the [Guix System GNU/Linux distribution](https://guix.gnu.org)
- Modify my [Scheme code](https://github.com/enzuru/guix-profiles) and run them to setup your own user
- Log into the user and you will be booted into the [exwm window manager](https://github.com/ch11ng/exwm)
