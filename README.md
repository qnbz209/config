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
    > set nobackup
    > set nowritebackup
    > set undofile
    >
    > set background=dark
    > syntax on
    >
    > highlight Normal guibg=#1E1E1E guifg=#D0D0D0
    >
    > highlight CursorLine guibg=#2B2B2B
    > highlight Visual guibg=#214283
    >
    > highlight LineNr guifg=#5C6370 guibg=#1E1E1E
    > highlight CursorLineNr guifg=#E8BF6A guibg=#2B2B2B
    >
    > highlight Comment guifg=#7F848E cterm=italic
    > highlight String guifg=#6A8759
    > highlight Constant guifg=#6897BB
    > highlight Keyword guifg=#CC7832
    > highlight Statement guifg=#CC7832
    > highlight Type guifg=#E8BF6A
    > highlight Function guifg=#9876AA
    > highlight Identifier guifg=#9876AA
    > highlight Number guifg=#6897BB
    >
    > highlight Conditional guifg=#CC7832
    > highlight Repeat guifg=#CC7832
    > highlight Operator guifg=#CC7832
    >
    > highlight MatchParen guifg=#FFFFFF guibg=#3C3F41
    > highlight Search guibg=#3C3F41 guifg=#E8BF6A
    > highlight IncSearch guibg=#E8BF6A guifg=#1E1E1E
    >
    > highlight StatusLine guibg=#3C3F41 guifg=#D0D0D0
    > highlight StatusLineNC guibg=#2B2B2B guifg=#7F848E
    >
    > highlight VertSplit guibg=#2B2B2B guifg=#3C3F41
    > highlight TabLine guibg=#2B2B2B guifg=#7F848E
    > highlight TabLineSel guibg=#3C3F41 guifg=#E8BF6A
    > highlight TabLineFill guibg=#1E1E1E
    >
    > highlight Pmenu guibg=#2B2B2B guifg=#D0D0D0
    > highlight PmenuSel guibg=#3C3F41 guifg=#E8BF6A
    > highlight Folded guibg=#2B2B2B guifg=#7F848E
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
- [Slack](https://slack.com/intl/ko-kr/downloads/mac)
- [iTerm2](https://iterm2.com/)
- [JetBrains IDEA](https://www.jetbrains.com/idea/)  

  > Use Temurin

- [JetBrains PyCharm](https://www.jetbrains.com/pycharm/)
- [VS Code](https://code.visualstudio.com/)
- [Postman](https://www.postman.com/downloads/)
- [Zoom](https://zoom.us/ko/download)
