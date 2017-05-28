Python.vim
==========

This is a set of menus/shortcuts to work with Python files. This work is kind
continuation of `Mikael Berthe script`_, with some improvements and fixes.

Installation
------------

To install it, any kind of Vim package manager can be used, like NeoBundle_,
Pathogen_, Vundle_ or vim-plug_.

For manual installation, copy subdirectories from this repository to your
``~/.vim`` directory.

Usage
-----

Default shortcuts are as follows:

- ``]]`` - jump to next class
- ``[[`` - jump to previous class
- ``}}`` - jump to next function or method
- ``{[`` - jump to previous function or method
- ``]t`` - jump to beginning of block
- ``]e`` - jump to end of block
- ``]<up>`` - jump to previous line with the same/lower indentation
- ``]<down>`` - jump to next line with the same/lower indentation
- ``]<`` - shift block to left
- ``]>`` - shift block to right
- ``]#`` - comment selection
- ``]u`` - uncomment selection
- ``vac`` - select (Visual Line Mode) current/previous class
- ``vaf`` - select (Visual Line Mode) current/previous function
- ``vab`` - select (Visual Line Mode) block

You can set the global variable ``g:py_select_leading_comments`` to 0
if you don't want to select comments preceding a declaration (these
are usually the description of the function/class).
You can set the global variable ``g:py_select_trailing_comments`` to 0
if you don't want to select comments at the end of a function/class.
If these variables are not defined, both leading and trailing comments
are selected.

If you use graphical version of vim (like gvim) you can access those options
through the menu called *Python*.

.. _Mikael Berthe script: http://www.vim.org/scripts/script.php?script_id=30
.. _Pathogen: https://github.com/tpope/vim-pathogen
.. _Vundle: https://github.com/gmarik/Vundle.vim
.. _NeoBundle: https://github.com/Shougo/neobundle.vim
.. _vim-plug: https://github.com/junegunn/vim-plug
