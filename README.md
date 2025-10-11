# Config

---

## Shell
- [Oh My Zsh](https://ohmyz.sh/#install)
- [powerlevel10k](https://devocean.sk.com/blog/techBoardDetail.do?ID=165667&boardType=techBlog)

---

## Package Managers
- [Homebrew](https://brew.sh/)
  - [Colima](https://keun.me/colima/) – Docker 대안
  - [NVM](https://formulae.brew.sh/formula/nvm) – Node Version Manager
  - [Yarn](https://formulae.brew.sh/formula/yarn) – 패키지 매니저
  - [Neovim](https://formulae.brew.sh/formula/neovim) – 텍스트 에디터

    > `~/.zshrc`
    > ```bash
    > alias n="nvim $1"
    > alias vi=nvim
    > alias vim=nvim
    > ```
    > `~/.vimrc`
    > ```bash
    > " line number
    > set nu
    > 
    > " not compatible with 'VI'. (required)'
    > set nocompatible
    > 
    > " Use ; for leader key (default : \\)
    > let mapleader=";"
    > 
    > " Tab space
    > set tabstop=4
    > 
    > " Indent space
    > set shiftwidth=4
    > 
    > " Tab key space
    > set softtabstop=4
    > 
    > " Backspace deletes tab space
    > set smarttab
    > 
    > " Tab -> space
    > set expandtab
    > 
    > " C language indent
    > set cindent
    > 
    > "highlight search on
    > set hlsearch
    > 
    > "incremental search on
    > set incsearch
    > 
    > "case sensitivity in search off
    > set nosmartcase
    > set visualbell
    > 
    > " Number of lines before bottom when scrolling vertically
    > set so=10
    > 
    > " backspace can delete anything
    > set backspace=indent,eol,start
    > set wildignore=*.o,*.obj,*.a,*.bak,*.exe,*~
    > 
    > " c: Auto-wrap comments,
    > " r: Auto insert the current comment leader after 'Enter'
    > " o: Auto insert the current comment leader after 'o' or 'O'
    > set formatoptions=cro
    > syn on
    > 
    > " coloring on the N'th column
    > set colorcolumn=80
    > set cursorline
    > 
    > "___highlight___
    > " ctermbg=235 -> dark grey
    > hi CursorLine       term=bold cterm=bold ctermbg=235
    > 
    > "___map___
    > "cure for backspace bug terminal
    > hi colorcolumn      ctermbg=235
    > imap ^? ^H
    > cmap ^? ^H
    > function! LoadVimFile(so_file)
    >     if filereadable(a:so_file)
    >         exe "so ".a:so_file
    >     endif
    > endfunction
    > autocmd BufReadPost *
    >   \ if line("'\"") > 0 && line("'\"") <= line("$") | exe "normal g`\"" | endif
    > 
    > " remap moving split tabs
    > vnoremap // y/<C-R>"<CR>
    > nnoremap <C-h> <C-w>h
    > nnoremap <C-j> <C-w>j
    > nnoremap <C-k> <C-w>k
    > nnoremap <C-l> <C-w>l
    > ```
    > ` ~/.config/nvim/init.vim`
    > ```bash
    > source ~/.vimrc
    > ```

---

## Docker
- [AWS CLI Docker](https://hub.docker.com/r/amazon/aws-cli)

  - `alias aws="docker run --rm -ti -v ~/.aws:/root/.aws amazon/aws-cli"`

---

## Applications
- [Google Chrome](https://www.google.com/intl/ko_kr/chrome/)

  > Some pages aren’t opening in Safari.

- [ChatGPT](https://chatgpt.com/ko-KR/download/)
- [Notion](https://www.notion.so/)
- [Notion Calendar](https://calendar.notion.so/)
- [Slack](https://slack.com/intl/ko-kr/downloads/mac)
- [iTerm2](https://iterm2.com/)
- [JetBrains IDEA](https://www.jetbrains.com/idea/)  

  > Use Temurin

- [JetBrains PyCharm](https://www.jetbrains.com/pycharm/)
- [VS Code](https://code.visualstudio.com/)
- [Postman](https://www.postman.com/downloads/)
- [Zoom](https://zoom.us/ko/download)
