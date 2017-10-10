## Watchout for
- [The Languages, Frameworks and Tools You Should Learn in 2017](http://tutorialzine.com/2016/12/the-languages-frameworks-tools-you-should-learn-in-2017/)


## Fun
- [Hype Driven Development](https://blog.daftcode.pl/hype-driven-development-3469fc2e9b22#.6yid21oth)


## Theory
- [Itsy Bitsy Data Structures](https://github.com/thejameskyle/itsy-bitsy-data-structures?utm_source=ESnextNews.com&utm_medium=Weekly+Newsletter&utm_campaign=2017-02-28)


## Management
- [Three Goals for Effective Backlog Management](https://spin.atomicobject.com/2017/06/14/effective-backlog-management-goals/)


## Books
- [DevFreeBooks](https://devfreebooks.github.io)


## Tools
- [The Bash Guide](http://guide.bash.academy)


## Git
- [Little Things I Like to Do with Git](https://csswizardry.com/2017/05/little-things-i-like-to-do-with-git/)
- [Conventional Commits](http://devboosts.com/2017/03/28/conventional-commits/)
- [Getting solid at Git rebase vs. merge](https://medium.com/@porteneuve/getting-solid-at-git-rebase-vs-merge-4fa1a48c53aa#.rt1xsmaft)
- [Git - When to Merge vs. When to Rebase](https://www.derekgourlay.com/blog/git-when-to-merge-vs-when-to-rebase/)
- [How to delete a Git branch both locally and remotely?](http://stackoverflow.com/questions/2003505/how-to-delete-a-git-branch-both-locally-and-remotely)
- [Git Tools - Credential Storage](https://git-scm.com/book/en/v2/Git-Tools-Credential-Storage)
- [Caching your GitHub password in Git](https://help.github.com/articles/caching-your-github-password-in-git/#platform-all)
- [Is there a way to skip password typing when using https://](http://stackoverflow.com/questions/5343068/is-there-a-way-to-skip-password-typing-when-using-https-on-github)
- [Bash Shortcuts to Enhance Your Git Workflow](https://medium.freecodecamp.com/bash-shortcuts-to-enhance-your-git-workflow-5107d64ea0ff#.h0rseziqm)
- [Git in 2016](https://hackernoon.com/git-in-2016-fad96ae22a15#.hftemdbv0)
- [A Small Matter of Programming](http://blog.wuwon.id.au/2010/09/painless-merge-conflict-resolution-in.html)
- [Git bisect](https://glebbahmutov.com/blog/git-bisect/)
- [Stop using `git pull`: A better workflow](https://adamcod.es/2014/12/10/git-pull-correct-workflow.html)
- [Try Git](https://try.github.io)
- [git - the simple guide](http://rogerdudler.github.io/git-guide/)
- [Learn Git Branching](http://learngitbranching.js.org)
- [Cheat Sheet](https://services.github.com/kit/downloads/github-git-cheat-sheet.pdf)
- [.gitignore files](https://github.com/github/gitignore)
- [Commit History](https://git-scm.com/book/en/v2/Git-Basics-Viewing-the-Commit-History)
- [Interactive Staging](https://git-scm.com/book/en/v2/Git-Tools-Interactive-Staging)
- [Stashing and Cleaning](https://git-scm.com/book/en/v2/Git-Tools-Stashing-and-Cleaning)
- [Searching](https://git-scm.com/book/en/v2/Git-Tools-Searching)
- [Reset Demystified](https://git-scm.com/book/en/v2/Git-Tools-Reset-Demystified)
- Rebase
  - [doc](https://git-scm.com/book/en/v2/Git-Branching-Rebasing)
  - [ref](https://git-scm.com/docs/git-rebase)
- [Advanced Merging](https://git-scm.com/book/en/v2/Git-Tools-Advanced-Merging)
- [Rewriting History](https://git-scm.com/book/en/v2/Git-Tools-Rewriting-History)
- [Revision Selection](https://git-scm.com/book/en/v2/Git-Tools-Revision-Selection)
- [Distributed Git - Contributing to a Project](https://git-scm.com/book/en/v2/Distributed-Git-Contributing-to-a-Project)
- [Distributed Git - Maintaining a Project](https://git-scm.com/book/en/v2/Distributed-Git-Maintaining-a-Project)
- Some commands
  - `git checkout -` will checkout the previous branch (shorthand for `git checkout @{-1}`)
  - `git rebase master --autostash` will stash and reapply stashed stuff after rebase
  - `git fetch origin --prune` fetches origin end cleans up a bit, removes deleted remote branches but not the checked out ones
  - `git config --global pull.rebase preserve` set pull to use rebase with preserve merges option
  - `git config --global rebase.autostash true`
  - `git config --global user.name "John Doe"`
  - `git config --global user.email johndoe@example.com`
  - `git config --global core.editor emacs`
  - `git config --global core.editor "'C:/Program Files (x86)/Notepad++/notepad++.exe' -multiInst -nosession"`
  - `git config --list` list git config in actual dir
  - `git config --global --list` list git global config
  - `git config user.name` check user name
  - `git config --global credential.helper cache` cache https auth temporarily
  - `git remote show origin` show remote info
  - `git tag -l "v1.8.5*"` search tags
  - `git tag -a v1.4 -m "my version 1.4"` create annnotated tag
  - `git tag -a v1.2 9fceb02` create annotated tag for prev commit
  - `git push origin v1.5` push a single tag
  - `git push origin --tags` push all tags
  - `git checkout -b version2 v2.0.0` "checkout" a tag
  - `git ls-remote [origin]` shows remote infos
  - `git remote show [origin]` shows remote detailed infos
  - `git push origin serverfix:awesomebranch` push to a branch with different name
  - `git checkout -b serverfix origin/serverfix` checkout remote tracking branch
  - `git checkout --track origin/serverfix` checkout remote tracking branch shorter
  - `git checkout serverfix` checkout remote tracking branch, shortest
  - `git branch -u origin/serverfix` setup local bracnch to track remote
    - `git branch --set-upstream-to origin/serverfix` setup local bracnch to track remote
  - `git merge @{u}` can be used instead `git merge origin/master`
    - `git merge @{upstream}` can be used instead `git merge origin/master`
  - `git branch -vv` check setup remote tracking branches
  - `git push origin --delete serverfix` delete remote branch serverfix
    - `git push origin :serverfix` delete remote branch serverfix
  - `git log master..head` to check commits what head has but master not, aslo `git rebase master` will reapply these commits
  - `git pull --rebase ` pull rebase instead pull merge
  - `git log --no-merges` check commit message structure/convention
  - `git request-pull origin/master myfork` create pull request info
  - `git format-patch -M origin/master` create a patch
  - `git apply /tmp/patch-ruby-client.patch` apply a patch
  - `git am 0001-limit-log-function.patch` apply a format-patch patch
  - `git log contrib --not master` exclude master commits from log smae as master..contrib
  - `git diff master...contrib` show only the new diffs introduced in contrib ?
  - `git log master...experiment` all commits which are reachable from master and experiment but not the common ones (eg: common ancestor, ...)
  - `git clean` clean/remove untracked/not ignored files (merge temp files, etc.)
  - `git clean -f -d` clean/remove untracked not/ignored files and empty dirs
  - `git clean -d -n` check what will be cleaned/removed
  - `git filter-branch --tree-filter 'rm -f passwords.txt' HEAD` removing a file from every commit

## Editor/IDE
- [Visual Studio Code](https://code.visualstudio.com/)
  - [Awesome VSCode](https://github.com/viatsko/awesome-vscode)
  - [Visual Studio Code treasures](https://medium.com/@0x1AD2/visual-studio-code-treasures-1accae07c60a)
  - [JavaScript Extensions Part 1](https://code.visualstudio.com/blogs/2016/09/14/js_roundup_1)
  - [JavaScript Extensions Part 2](http://code.visualstudio.com/blogs/2016/10/31/js_roundup_2)
  - Extensions
    - [Quick and Simple Text Selection](https://marketplace.visualstudio.com/items?itemName=dbankier.vscode-quick-select)
    - [Prettier - JavaScript formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
    - [JavaScript Standard Style](https://marketplace.visualstudio.com/items?itemName=chenxsan.vscode-standardjs)
    - [JavaScript standardjs styled snippets](https://marketplace.visualstudio.com/items?itemName=capaj.vscode-standardjs-snippets)
    - [PowerShell](https://marketplace.visualstudio.com/items?itemName=ms-vscode.PowerShell)
    - [Sublime Babel ](https://marketplace.visualstudio.com/items?itemName=joshpeng.sublime-babel-vscode)
    - [Babel ES6/ES7](https://marketplace.visualstudio.com/items?itemName=dzannotti.vscode-babel-coloring)
    - [JavaScript (ES6) code snippets](https://marketplace.visualstudio.com/items?itemName=xabikos.JavaScriptSnippets)
    - [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
    - [TSLint](https://marketplace.visualstudio.com/items?itemName=eg2.tslint)
    - [Auto Import](https://marketplace.visualstudio.com/items?itemName=steoates.autoimport)
    - [Auto Close Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-close-tag)
    - [Auto Rename Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag)
    - [Git Project Manager](https://marketplace.visualstudio.com/items?itemName=felipecaputo.git-project-manager)
    - [Git History (git log)](https://marketplace.visualstudio.com/items?itemName=donjayamanne.githistory)
    - [Git Blame](https://marketplace.visualstudio.com/items?itemName=waderyan.gitblame)
    - [HTMLHint](https://marketplace.visualstudio.com/items?itemName=mkaufman.HTMLHint)
    - [HTML CSS Class Completion](https://marketplace.visualstudio.com/items?itemName=Zignd.html-css-class-completion)
    - [HTML Snippets](https://marketplace.visualstudio.com/items?itemName=abusaidm.html-snippets)
    - [Sass](https://marketplace.visualstudio.com/items?itemName=robinbentley.sass-indented)
    - [Visual Studio Code Settings Sync ](https://marketplace.visualstudio.com/items?itemName=Shan.code-settings-sync)
    - [Project Manager](https://marketplace.visualstudio.com/items?itemName=alefragnani.project-manager)
    - [Bookmarks](https://marketplace.visualstudio.com/items?itemName=alefragnani.Bookmarks)
    - [beautify](https://marketplace.visualstudio.com/items?itemName=HookyQR.beautify)
    - [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
    - [npm Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.npm-intellisense)
    - [Vetur](https://marketplace.visualstudio.com/items?itemName=octref.vetur) [vue]
    - [Reactjs code snippets](https://marketplace.visualstudio.com/items?itemName=xabikos.ReactSnippets) [react]
    - [jsx](https://marketplace.visualstudio.com/items?itemName=TwentyChung.jsx) [react]
    - [Angular 2 TypeScript + HTML Snippets](https://marketplace.visualstudio.com/items?itemName=UVBrain.Angular2) [angular]
    - [language-vscode-javascript-angular2](https://marketplace.visualstudio.com/items?itemName=nwallace.language-vscode-javascript-angular2) [angular]

- [Sublime Text](https://www.sublimetext.com/)
  - dotfiles
    - [PackageControl Syncing](https://packagecontrol.io/docs/syncing)
  - [PackageControl](https://packagecontrol.io)
  - [15 Awesome Sublime Text Plugins For Web Development](http://tutorialzine.com/2016/10/15-awesome-sublime-text-plugins-for-web-development/)
    - [Babel](https://packagecontrol.io/packages/Babel)
      - [Babel Snippets](https://packagecontrol.io/packages/Babel%20Snippets)
    - [Java​Script & Node​JS Snippets](https://packagecontrol.io/packages/JavaScript%20%26%20NodeJS%20Snippets)
    - [Emmet](https://packagecontrol.io/packages/Emmet)
    - [TypeScript](https://packagecontrol.io/packages/TypeScript)
    - [Angular](https://packagecontrol.io/packages/AngularJS)
    - [SublimeLinter](https://packagecontrol.io/packages/SublimeLinter)
      - [Sublime​Linter-contrib-eslint](https://packagecontrol.io/packages/SublimeLinter-contrib-eslint)
      - [Sublime​Linter-json](https://packagecontrol.io/packages/SublimeLinter-json)
      - [Sublime​Linter-csslint](https://packagecontrol.io/packages/SublimeLinter-csslint)
    - [ESLint-Formatter](https://packagecontrol.io/packages/ESLint-Formatter)
    - [Sublime​Code​Intel](https://packagecontrol.io/packages/SublimeCodeIntel)
    - [SideBarEnhancements](https://packagecontrol.io/packages/SideBarEnhancements)
    - [Color Highlighter](https://packagecontrol.io/packages/Color%20Highlighter)
    - [Placeholders](https://packagecontrol.io/packages/Placeholders)
    - [Advanced​New​File](https://packagecontrol.io/packages/AdvancedNewFile)
    - [Git](https://packagecontrol.io/packages/Git)
    - [GitGutter](https://packagecontrol.io/packages/GitGutter)
  - [Markdown​Editing](https://packagecontrol.io/packages/MarkdownEditing)
  - [Markdown Preview](https://packagecontrol.io/packages/Markdown%20Preview)
  - Color Schemes
    - [Monokai Extended](https://packagecontrol.io/packages/Monokai%20Extended)
  - ColorSublime
  - PackageDev
  - ScopeHunter

- [Atom](https://atom.io/)
  - [Nuclide](https://nuclide.io/)

- [ALM Tools](http://alm.tools/)
- [Brackets](http://brackets.io/)
