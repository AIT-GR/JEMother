# JEMother
git repo with submodules to build the whole JEVis suit

automatically initialize and download the repository including the submodules with the command

`git clone --recursive https://github.com/AIT-JEVis/JEMother.git`

To pull changes for JEMother and all submodules and then checkout the (by JEMother) specified commits we reccomend to define a git-alias:

`git config alias.pullall '!f(){ git pull "$@" && git submodule update --init --recursive; }; f'`

and then instead of just `git pull` use `git pullall`

To update all submodules to latest upstream-commit use

`git submodule update --remote --merge`

