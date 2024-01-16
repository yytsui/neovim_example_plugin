This is an example showing how to develope a neovim pluign with lua with 3rd party dependencies.
(source)[https://www.linode.com/docs/guides/write-a-neovim-plugin-with-lua/]
And.
1. Assuming this directory is under /tmp/h/
2. install PLUG
    % curl -fLo ~/.local/share/nvim/site/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
3. clone 3rd partyy Lua library
    % cd ./lua
    % git clone https://github.com/stepelu/lua-ljsqlite3.git ljqlite3
    % git clone https://github.com/stepelu/lua-xsys.git xsys

4. content of ~/.config/nvim/init.vim
"""
call plug#begin('~/.local/share/nvim/site/autoload/plug.vim')
Plug '/tmp/h/example-plugin'
call plug#end()
"""
~
