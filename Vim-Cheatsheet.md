Vim Cheat Sheet
===============
- `<C-o>`    move to a previous cursor
- `<C-i>`    move to a forward cursor
- `<C-]>`    jump to first tag ocurrence. Cycle with tpope/unimpared ]t [t
- `<C-t>`    jump to first item in the tagstack
- `gv`       rehighlights the last selection
- `gb`       rehighlights the last pasted text (custom mapping)
- `g&`       repeat last substitute preserving flags
- `gw`       reformat line according textwidth
- `gi`       go to last insertion and switch to insert mode
- `<C-n|p>`  Word wise completion
- `<C-x-l>`  Line wise completion
- `<C-x-f>`  File wise completion
- `<C-x-k>`  Dictionary completion
- `<C-x-o>`  Omni completion
- `<C-x-u>`  User custom completion
- `:vs#`     split and open the alternate file
- `cgn`      Change visual selection (repeteable)
- `<C-x-e>`  In bash, open $EDITOR with current command line

Spell checking
==============
- `[s`       move to previous misspelled word
- `]s`       move to next misspelled word
- `z=`       show alternatives to correct misspelled

Searching
=========
- `:%s/\v(very magic)/\1/gc` very magic mode
- `<c-r><c-w>`  insert word under cursor
- `<c-r>/`      insert last search pattern
- `<c-r>0`      insert last yank

Bookmarks
=========
- `ma`     set mark 'a' to current position
- ``a`     go to mark 'a'
- ``.`     go to last change mark
- ``^`     mark to go to last insertion
- `g;|g,`  go forward/backward through the changelist
- `:marks` show all available marks

Files
=====
- `:e!`        reload current file discarding changes
- `:r [file]`  insert content of file
- `:r !date`   insert the results from command

Diff
====
- `do`                get changes from other window into current one
- `dp`                put changes from current window into other one
- `]c`                jump to the next change
- `[c`                jump to the previous change
- `:windo diffthis`   activate vimdiff in splitted window
- `:windo diffoff`    deactivate vimdiff mode
- `:diffupdate`       update diff color (useful after undo operation)

What to do on a vim -u NONE -N?
============================
- `:set path=**`                sets the path to cwd and recursively
- `:set path=**,other/**`       comma separated list of paths
- `:set suffixesadd=.java,.py`  use this to avoid extension when using find
- `:find somefile`              finds somefile in path
- `:syntax on`                  activate syntax highlighting
- `:set wildmode=full`          gives you autocompletion (try with find!)
- `:set wildmenu`               to show in a menu the autocompletion
- `:set wildignore=*.pyc,...`   ignore certain filetypes when autocompleting
- `:ls`                         list buffers
- `:Explore`                    use builtin exlorer instead of NERDTree