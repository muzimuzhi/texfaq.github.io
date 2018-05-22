# Contributing to the FAQ

Thanks for considering contributing to the TeX FAQ: feedback, fixes and ideas are
all useful.

## ChangeLog and commit messages

Please not any significant change to the content of questions in
`CHANGELOG.md`, including which question is changed in the format `Q-<name>`.

Commit messages where the content of a single question is changed should start
with `Q-<name>`.

## Formatting

The online TeX FAQ is written in [GitHub-flavoured
Markdown](https://guides.github.com/features/mastering-markdown/), and uses the
[GitHub Pages](https://pages.github.com/) system to convert this to web pages.
In general, Markdown is easy to use, and offers enough formatting power to make
the FAQ useful. There are a few things to watch out for

- The Jekyll 'back-end' used by GitHub Pages is somewhat picky about unbalanced
  braces (`{` and `}`), even in code blocks. That's because it is looking for
  some instructions of it's own there. To turn this off, surround the relevant
  parts of your source with
  ```
  <!-- {% raw %} -->
  ```
  and
  ```
  <!-- {% endraw %} -->
  ```
  (Typically these will go just before and after the <code>```</code> lines.)

- Only use block quotes for real quotations: use code markup for terminal
  output and similar
