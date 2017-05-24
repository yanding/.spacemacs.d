[![Built with Spacemacs](https://cdn.rawgit.com/syl20bnr/spacemacs/442d025779da2f62fc86c2082703697714db6514/assets/spacemacs-badge.svg)](http://spacemacs.org)

<hr>

# .spacemacs.d
My `.spacemacs.d` directory as a [Spacemacs](https://github.com/syl20bnr/spacemacs)
configuration. It's optimized for English and Thai languages.

# What is [Spacemacs](https://github.com/syl20bnr/spacemacs) ?
**Spacemacs** is an **Emacs** configuration distribution that
makes [Emacs](https://github.com/emacs-mirror/emacs) behave a lot
like [Vim](https://github.com/vim/vim) by using modal text editing and also
provides many useful features out of the box.

Its four core pillars are *Mnemonic*, *Discoverable*,
*Consistent* and *"Crowd-Configured"*.

It forces heavy usage of **space** bar, thus the name **Spacemacs**. It refers
to the space bar as `SPC`. The purpose of using space bar is to reduce numbers
of `Ctrl`, `Alt`, `Shift` combinations. It's good for your pinky finger and your
editing speed. It also lowers the risk
of [RSI](https://en.wikipedia.org/wiki/Repetitive_strain_injury).

# Screenshots
These are screenshots taken over time. The most recent one is at the bottom.

My current theme is **material** (I switched back from **majapahit-dark**). And
I've also reduced that too much colorful identifiers to colorize only variables.
The commit that did just that is [48613a90373651de2a54fd5f5fc6c6371241b32c](https://github.com/off99555/.spacemacs.d/commit/48613a90373651de2a54fd5f5fc6c6371241b32c).
You can revert it if you want.

This is a **Spacemacs** instance on Windows 10 with **material** theme showing **which
key** buffer that is invoked by pressing `SPC`.
[![2016-12-12_23-42-18.png](screenshots/2016-12-12_23-42-18.png)
](screenshots/2016-12-12_23-42-18.png?raw=true)

This is another **Spacemacs** instance on Windows 10 with **majapahit-dark** theme
showing **magit** package and the **Spacemacs** home buffer.
[![2016-12-13_21-35-23.png](screenshots/2016-12-13_21-35-23.png)
](screenshots/2016-12-13_21-35-23.png?raw=true)

This shows **magit log** and **helm** buffer list. It also shows the
**markdown-mode buffer**.
[![2016-12-22_21-02-07.png](screenshots/2016-12-22_21-02-07.png)
](screenshots/2016-12-22_21-02-07.png?raw=true)

This shows **nerdtree** on the left with file icons package. It can be toggled
using `SPC f t`
[![2016-12-22_21-05-25.png](screenshots/2016-12-22_21-05-25.png)
](screenshots/2016-12-22_21-05-25.png?raw=true)

Want to use CLI? Here is a python interactive shell inside Emacs, you can send a
piece of code to it and use it as usual. I also show the **eshell** on the
bottom corner which is Emacs' own shell that can do Unix stuff inside Windows as
well!
[![2017-02-28_14-13-37.png](screenshots/2017-02-28_14-13-37.png)
](screenshots/2017-02-28_14-13-37.png?raw=true)


# Installation
1. Install [Spacemacs](https://github.com/syl20bnr/spacemacs/tree/develop) from
  develop branch. Follow the instruction for installation and don't forget to
  install dependencies like fonts.

2. Clone this repository into your home.
  `git clone https://github.com/off99555/.spacemacs.d.git`

3. Remove `.spacemacs` file inside your home.
  It's a file automatically generated by **Spacemacs**.
  `rm .spacemacs`

4. That's it!

  You are now ready to use **Spacemacs** with my configuration. For the best
  experience, use **Spacemacs** on a graphical version of Emacs!

# Dependencies
- I highly recommend using
  [Source Code Pro](http://store1.adobe.com/cfusion/store/html/index.cfm?event=displayFontPackage&code=1960) font
  from Adobe (it's free and awesome font for writing and programming). My
  configuration is already setup to try to use it. You can download it freely
  from this repository:
  [https://github.com/adobe-fonts/source-code-pro](https://github.com/adobe-fonts/source-code-pro)
- [all-the-icons](https://github.com/domtronn/all-the-icons.el/tree/master/fonts) fonts
  are needed for `SPC f t` (neotree) to display file icons properly. Go download
  all **.ttf** files there.
- Search tools like "[rg](https://github.com/BurntSushi/ripgrep)",
  "[ag](https://github.com/ggreer/the_silver_searcher)",
  "[pt](https://github.com/monochromegane/the_platinum_searcher)", "ack", or
  "grep". You only need to install one of them. I recommend "ag" the as I'm
  happy with it. On Windows, you can install **ag** the simplest way
  using [chocolatey](https://chocolatey.org/). Run `choco install ag` and you
  are good to go. If you want, you can also use **rg** or **pt** instead. They both are
  easy to install and have similar performance. Don't forget to add its
  directory to your **PATH** variable, otherwise **Spacemacs** wouldn't know where
  to locate the searcher.

# Configurations
Edit `~/.spacemacs.d/init.el` instead of `~/.spacemacs`.

You can open the configuration file directly via `SPC f e d`.

You can also compare the differences betweeh the default **Spacemacs** settings
versus mine via `SPC f e D`.

# Learning to Use Spacemacs
If you know **Vi**, you will be able to use **Spacemacs** without much of a hassle.
But if you don't, you can press `SPC h T` to open the **Evil mode** interactive
tutor so that you can learn enough **Vi** keybindings to survive in **Spacemacs**.

**NOTE:** **Evil mode** is an **Emacs** package that tries to mimic **Vi**.

After you have familiarized yourself with **Evil** modal editing, your next
station is to discover **Spacemacs**' features. You can do so in several ways.

By hitting `SPC ?` you can search for functions that have certain keybindings
attached. You can learn what key does what and what function is assigned to
which key this way.

The biggest help is probably `SPC h SPC`. It lists all **Spacemacs layers** and
packages documentation. The very first document that you should read is named
*BEGINNERS_TUTORIAL.ORG*. Read it first to familiarize yourself with **Spacemacs**.

If things go wrong, you can always press `ESC` or `Ctrl-g` to escape out of
frustration.

## [OPTIONAL] Using Emacs keybindings instead of Vi
If you are an **Emacs** enthusiast, you can switch to use **Emacs** keybindings.
**Emacs** keybindings mode in **Spacemacs** is called a **Holy mode**.
You can toggle between the **Holy mode** and the **Evil mode** by pressing `Ctrl-z`.

But really, who love **Emacs**'s weird keybindings that says *"Ctrl this, Ctrl
that"* all the time anyway?

Everyone loves **Vi** keybindings. ([Unless](http://stackoverflow.com/questions/1218390/what-is-your-most-productive-shortcut-with-vim/1220118#1220118) you do
not [grok](https://en.wikipedia.org/wiki/Grok) **Vi**)
So, try to master **Vi** keybindings and it will be beneficial to you.
If you want to execute the next command in **Holy mode**, you can use `\` key in
**evil normal state** which is similar to **Vi**'s normal mode.

## Cool stuff you can do inside Spacemacs
Before you do any of this stuff, please read the *BEGINNERS_TUTORIAL.ORG* first.
Because the way this section is written is assuming that you understand
**Spacemacs**' core concepts already.

- You can open and view images inside Spacemacs.
- Type `SPC '` to open a shell buffer (specifically **eshell**).
- Type `SPC /` to do a smart search inside the project using the search tool you
  preferred in the *Dependency* section.
- Type `SPC x g t` to translate a word under point using Google translate (the
  language is currently set from English to Thai).
- Type `SPC x l s` to sort selected lines or the entire buffer
- Type `SPC s w g` to search using Google.
- Type `SPC s s` to search interactively inside current buffer. To edit all the
  matching results, type `C-c C-e` next and do your editing there.
- Type `SPC s e` to activate **iedit** on the current symbol or visually
  selected text. You can then edit this symbol and it will affect all
  occurences inside the buffer.
- Type `SPC g l l` to open current file on **GitHub** in your default web
  browser. (If the file you are on is inside a **git** repository)
- Type `SPC g s` to open a git status of your current file inside **magit**.
  You can discover more actions by typing `?` next.
- Type `SPC g f h` to open current file's history using **magit** log.
- Type `SPC f j` or `SPC j d` to jump to a file using **dired-mode**.
- Type `SPC j i` to jump to a function using **helm imenu**
- Type `SPC j j` followed by a character to jump to a character inside all
  display window using **avy**.
- Type `SPC j u` to jump to a URL inside all display window using **avy**.
- Type `SPC b i` to to open **imenu list** (a symbol index).
- Type `SPC b s` to open a scratch buffer you can play with immediately.
- Type `SPC f J` to open a new junk file that you can save and abandon later.
- Type `SPC TAB` to toggle between the current buffer and the lastly visited buffer.
- Type `SPC SPC` to execute an **Emacs** command.
- Type `SPC i s` to insert a snippet using **yasnippet**.
- Type `SPC i e` to insert an emoji.
- Type `SPC i l l` to insert a random *lorem ipsum* placeholder text.
- Type `SPC r y` to see all the previously yanked text inside the **kill ring**.
- Type `SPC T F` or `F11` to toggle fullscreen.
- Type `SPC w u` or `SPC w U` to use **winner** to undo/redo window configurations.
- Type `SPC w m` to toggle maximize current window.
- Type `SPC w f` to toggle follow mode in the current buffer. You can then type
  `SPC w v` to split a new window vertically. The new window will show the same
  buffer BUT with a little twist. Put simply, if your window on the left shows
  line 1 - 50 then your window on the right will show line 51 - 100. It also
  sync motion on both buffers, try it and you will love it!
- Type `SPC w c` to toggle centered-buffer-mode. Have you ever felt like your
  screen is really wide but your text buffer is only consuming half left of your
  screen leaving the half right empty without purpose? If so, try using this
  command!
- Type `SPC v` then `v` repeatedly to expand selection on the region like in
  [IntelliJ IDEA](https://www.jetbrains.com/idea/)'s `C-w` feature.
- Type `SPC a u` to visualize your undo history as a tree
- Type `SPC a E` to open an emoji cheatsheet buffer
- Type `fd` quickly to quit out of almost everything. You can exit evil insert
  state, evil visual state, helm mode, holy mode, iedit mode, etc. If you are a
  veteran **Vim** user and have it set to `jk` then learn to change your habit
  because setting this key to `jk` can quit from the visual state accidentally
  when moving up or down a line.

  If the thing you are trying to quit out of is a **minibuffer**, just press `q`
  to quit it.

## Cool Emacs keys
**Emacs** keybindings can also be nice sometimes. So, instead of hating it. We
should appreciate its good parts and abandon its ugliness.
But most of these keys are also available using `SPC` key too.

- Type `M-q` to toggle between filling or not filling the current paragraph.
  (Wrapping text on to new lines)
- Type `M-t` to transpose current word with the previous word. If the point is
  not on the first character of the word then it will transpose current word
  with the next word instead.
- Type `M-u` to upper case the next word.
- Type `M-l` to lower case the next word.
- Type `M-a` to go to the previous sentence similar to `(` but not exactly the same.
- Type `M-e` to go to the next sentence similar to `)` but not exactly the same.
- Type `M-SPC` to retain only one space if there are many spaces. If there are
  no spaces, it will insert one before the point.
- Type `M-k` to kill from point to end of sentence
- Type `M-;` to insert a comment symbol. if the comment already exists, jump to
  it instead.
- Type `M-h` to put point at beginning of this paragraph, mark at end. Similar
  to `vap` in **Evil** mode.
- Type `C-/` or `C-_` to undo changes similar to `u` but works inside **Evil
  insert state** too.

## Tips for Thai people
You can learn some basic **Vim** keys from this [website](https://vim.rtorr.com/lang/th/).
Then you can apply it inside **Evil mode** wonderfully.

**Emacs** have a
[Thai utility package](https://github.com/emacs-mirror/emacs/blob/master/lisp/language/thai-util.el) 
available into the core by default. It understands Thai language using a decent
algorithm with
[a big list of Thai words](https://github.com/emacs-mirror/emacs/blob/master/lisp/language/thai-word.el).
It's not something you would find in **Vim**.

Press `SPC SPC` then `thai-word-mode` to toggle Thai word mode. This will alter
the key `M-f`, `M-b`, `M-d`, `C-DEL`, `M-t` to understand Thai words.
See [thai-util.el](https://github.com/emacs-mirror/emacs/blob/master/lisp/language/thai-util.el) 
if you are curious about how it works.
