Follow My Lead
==============
Vim plugin for showing all your `<Leader>` mappings in a readable table including the descriptions.

Installation
------------
Copy `plugin/follow-my-lead.vim` to `~/.vim/plugin`

Or add a GitHub repository entry if you are using a Plugin Manager such as `Vundle`:

```vim
Plugin 'ktonga/vim-follow-my-lead'
```

or `Pathogen`:

Get pathogen

```mkdir -p ~/.vim/autoload ~/.vim/bundle && \
curl -LSso ~/.vim/autoload/pathogen.vim https://tpo.pe/pathogen.vim```

clone repository

```(cd ~/.vim/bundle && git clone https://github.com/ktonga/vim-follow-my-lead/edit/master/README.md)```

Features
--------
* Look for mappings (only to `<Leader>`) in scripts sourced by Vim
* By default only `.vimrc` is used. It honours `$MYVIMRC` variable.
* All sourced vim scripts can be used if specified by configuration (see Options)
* If the line previous to the mapping is a comment it will be used as the description
* Mappings are shown in a table with the following columns
  * Mode: which mode the mapping applies to
  * LHS: left hand side of the mapping (without `<Leader>`)
  * Description: The mapping comment if present

Screenshots
-----------
![FML screenshot](http://drive.google.com/uc?export=download&id=0BxOk4ZkCuP9uUV9WbktDSV9fSG8)

Shortcuts
---------
* `<Leader>fml`: Default mapping for triggering the plugin. It shows the mapping in a vertical split
* `q`: Closes the mappings window

Options
-------
* `g:fml_all_sources`: if `1` all sources are used, if `0` just `$MYVIMRC` is used. Default `0`
* _More options comming soon_

License
-------

Copyright (C) 2015 Gaston Tonietti

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
