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
    > ```
    > set nocompatible
    > set number
    > set tabstop=4
    > set shiftwidth=4
    > set softtabstop=4
    > set expandtab
    > set smarttab
    > set cindent
    > set hlsearch
    > set incsearch
    > set nosmartcase
    > set backspace=indent,eol,start
    > set scrolloff=10
    > set wildignore=*.o,*.obj,*.a,*.bak,*.exe,*~
    >
    > let mapleader=";"
    >
    > set cursorline
    >
    > set formatoptions=cro
    >
    > nnoremap <C-h> <C-w>h
    > nnoremap <C-j> <C-w>j
    > nnoremap <C-k> <C-w>k
    > nnoremap <C-l> <C-w>l
    > vnoremap // y/<C-R>"<CR>
    >
    > autocmd BufReadPost *
    >   \ if line("'\"") > 0 && line("'\"") <= line("$") |
    >   \ exe "normal g`\"" |
    >   \ endif
    >
    > hi CursorLine cterm=NONE ctermbg=236 guibg=#323232
    > hi Visual cterm=NONE ctermbg=24 guibg=#214283
    > hi Search ctermfg=0 ctermbg=214 guifg=#1e1e2e guibg=#ffcc66
    > hi IncSearch ctermfg=0 ctermbg=214 guifg=#1e1e2e guibg=#ffcc66
    > hi Comment ctermfg=59 gui=italic guifg=#808080
    > hi Constant ctermfg=215 guifg=#ff9e64
    > hi Identifier ctermfg=75 guifg=#7aa2f7
    > hi Function ctermfg=75 guifg=#7aa2f7
    > hi Keyword ctermfg=214 guifg=#ff9e64
    > hi Type ctermfg=108 guifg=#9ece6a
    > hi Todo ctermfg=0 ctermbg=214 gui=bold guifg=#1e1e2e guibg=#ffcc66
    >
    > set nobackup
    > set nowritebackup
    > set undofile
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
