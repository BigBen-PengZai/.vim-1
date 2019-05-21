# .vim

## After Installation, You Need To:


## After Installation, You Might Want To:

### On MacOS:

- [ ] Install MacVim and use Iterm2 if something is not working right

### For Error Checking
- [ ] See `_machine_specific.vim`

### For Code AutoComplete (YouCompleteMe)

- [ ] Install `cmake`
- [ ] Run `sudo python3 [your vim folder]/plugged/install.py`
- [ ] For python: `sudo pip3 install pylint autopep8 yapf`

### For Taglist:

- [ ] Install `ctags` for function/class/variable list


## Keyboard Shortcuts for `NORMAL` (`COMMAND`) Mode

### 1 Basic Commands

#### 1.1 The Most Basics

**`k`** : to switch to **`INSERT`** : mode, equals to key `i`

**`Q`** : quit current vim window, equals to command `:q`

**`S`** : save the current file, equals to command `:s`

**_IMPORTANT_**

  Since the `i` key has been mapped to `k`, every command (combination) that involves `i` should use `k` instead (for example, `ciw` should be `ckw`).

#### 1.2 Cursor Movement

| Command    | What it does                                              | Equivalent (QWERTY) |
|------------|-----------------------------------------------------------|---------------------|
| `u`        | cursor up a terminal line                                 | `gk`                |
| `e`        | cursor down a terminal line                               | `gj`                |
| `n`        | cursor left                                               | `h`                 |
| `i`        | cursor right                                              | `l`                 |
| `U`        | cursor up 5 terminal lines                                | `5gk`               |
| `E`        | cursor down 5 terminal lines                              | `5gj`               |
| `N`        | cursor to the start of the line                           | `0`                 |
| `I`        | cursor to the end of the line                             | `$`                 |
| `Ctrl` `u` | move the view port up 5 lines without moving the cursor   | `Ctrl` `y`          |
| `Ctrl` `e` | move the view port down 5 lines without moving the cursor | `Ctrl` `e`          |

#### 1.3 Some Other Commands That Your Moms Don't Tell You

| Command | What it does                       |
|---------|------------------------------------|
| `<C-i>` | Go to the next cursor position     |
| `<C-o>` | Go to the previous cursor position |

### 2 Window Management

#### 2.1 Creating Window Through Split Screen

**`su`** : Create a new horizontal split screen and place it above the current window

**`se`** : Create a new horizontal split screen and place it below the current window

**`sn`** : Create a new vertical split screen and place it left to the current window

**`si`** : Create a new vertical split screen and place it right to the current window

#### 2.2 Moving the Cursor Between Different Windows

| Action                         | Shortcut   | Command  |
|--------------------------------|------------|----------|
| Move cursor to the next window | `<SPACE>w` | `<C-w>w` |

### 3 NERDTree

| Action          | Shortcut | Command           |
|-----------------|----------|-------------------|
| Toggle NerdTree | `tt`     | `:NERDTreeToggle` |

#### 3.2 Navigating in NERDTree

### 4 AutoComplete (YCM)

| Action            | Shortcut | Command                                           |
|-------------------|----------|---------------------------------------------------|
| Go to definition  | `gd`     | `:YcmCompleter GoToDefinitionElseDeclaration<CR>` |
| Get documentation | `g/`     | `:YcmCompleter GetDoc<CR>`                        |
| Get type          | `gt`     | `:YcmCompleter GetType<CR>`                       |
| Go to references  | `gr`     | `:YcmCompleter GoToReferences`                    |

### 5 Bookmarks (vim-bookmarks)

| Action                              | Shortcut | Command                 |
|-------------------------------------|----------|-------------------------|
| Add/remove bookmark at current line | `mm`     | `:BookmarkToggle<CR>`   |
| Add/edit/remove annotation          | `mm`     | `:BookmarkAnnotate<CR>` |
| Jump to the next bookmark in buffer | `mn`     | `:BookmarkNext<CR>`     |
| Jump to the previous bookmark       | `mp`     | `:BookmarkPrev<CR>`     |

For more commands, see [here](https://github.com/MattesGroeger/vim-bookmarks#usage)

### 6 Markdown File Editing

#### 6.1 Edit Table with `vim-table-mode`

Toggle "Table Editing Mode" with `<SPACE>` (equals to command `:TableModeToggle<CR>`)
