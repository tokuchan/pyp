e-pyp
=====

Welcome to *e-pyp*, an *extended* or *experimental* `pyp`. The original, from
which this project is forked, can be found here: code.google.com/p/pyp. I do
not mean, in any way, to detract from it. This project merely offers a view of
several possibilities.

Why Did I Fork `pyp`
====================

Technically, this is a fork of the original `pyp` project. Actually, I want to
get my features cleaned up and stable enough for them to be included in the
official version. So, it might be best to think of this version as a preview of
possibilities, rather than competition with the original.

What Features are Offered?
==========================

*e-pyp* currently offers the following features, with more to come:

1. `pyp` now offers regex match notation. So, to match input against a regex,
   you can use `/pattern/`. Even better, any matching groups in your pattern
   become entries in a list. So, you can use a regex to chunk input, just like
   `u`, `m`, `a`, and friends, but with any pattern!

What Features are Planned?
==========================

*e-pyp* doesn't *yet* offer these features, but they are in the works:

1. Every string is a format call in disguise. Since every pipe in `pyp` has an
   input, and sometimes those inputs are lists, it seems natural for naked
   strings to be turned into `format` calls. So, a pattern like this: `pyp
   "u|'{}: {}'"`, would split the input on underscores, then print the first
   element, followed by colon, followed by the second element.

1. Clipboard as source and destination. It seems natural to have a `clip` magic
   variable in `pyp`. When you pipe from it, you get whatever is in the
   clipboard, including `None` if its empty. When you pipe to `clip` your input
   is sent to the clipboard for you. This gives `pyp` a nice way to interact
   with other, especially GUI, programs.

1. Docopt support. `pyp`, unlike PERL, has no way for users to add
   configuration to canned macros and pyp scripts. In PERL, rudimentary
   switches are enabled with the `-r` argument. I want to offer more. In `pyp`,
   if you send a string to the `options` target, you can configure options
   parsing. When you pipe from `options`, you will get a parsed dictionary
   with your options in it. For more details on the string's format, see
   the docopt project.

Contributing to the Project
===========================

If you can, you should try to contribute to the original `pyp` project, but if
you'd like to send me a pull request, please read the CONTRIBUTING file first.
