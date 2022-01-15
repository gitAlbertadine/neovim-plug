# neovim-plug
```

https://github.com/junegunn/vim-plug
-neovim:
sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
mkdir nvim
vim ~/.config/nvim/init.vim
__----_-------
autocmd FileType javascript setlocal formatprg=prettier\ --single-quote\ --trailing-comma\ es5
autocmd BufWritePre,TextChanged,InsertLeave *.js Neoformat
" Use formatprg when available
let g:neoformat_try_formatprg = 1
call plug#begin('/data/data/com.termux/files/home/.local/share/nvim/site/plugged')
Plug 'isruslan/vim-es6'
Plug 'sbdchd/neoformat'
call plug#end()
-----====-=-=--
https://prettier.io/docs/en/vim.html

```
