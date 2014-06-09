salazarpardo.github.io
======================

Lea Verou generally mirrors master branch changes to gh-pages, and covers the workflow in Easily keep gh-pages in sync with master. Do this by replacing the git checkout master and second git commit commands with git rebase master:

$ git add .
$ git status // to see what changes are going to be committed
$ git commit -m 'Some descriptive commit message'
$ git push // push the master branch changes to GitHub
$ git checkout gh-pages // go to the gh-pages branch
$ git rebase master // bring gh-pages up to date with master
$ git push // push the gh-pages branch changes to GitHub Pages
$ git checkout master // return to the master branch
