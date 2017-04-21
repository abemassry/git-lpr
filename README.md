# git-lpr
*List open PRs on GitHub*

`git lpr` lists open PRs on GitHub for the local origin branch

## INSTALL
1. make a ~/bin directory if it doesn't already exist

  `mkdir ~/bin`

2. add ~/bin to your PATH in your .bashrc / .zshrc / ... if it's not
   already there
   
  `export PATH=~/bin:$PATH`

3. copy git-lpr to your ~/bin directory

  `cp git-lpr ~/bin`

## Usage
`git lpr` lists PRs

### Output List (example)
```
1 https://github.com/smbaker/pynest/pull/20   adding a etst fgiler
2 https://github.com/smbaker/pynest/pull/19   Add &#39;mode&#39; command to turn thermostat on and off
3 https://github.com/smbaker/pynest/pull/18   Force TSLv1 to allow connection to be made correctly
4 https://github.com/smbaker/pynest/pull/14   Update to Use Print Correctly
5 https://github.com/smbaker/pynest/pull/10   adding setmode and show mode
6 https://github.com/smbaker/pynest/pull/9   Make pynest installable via pip, split pynest.py into an main program and a library, and move from urllibX to requests
7 https://github.com/smbaker/pynest/pull/8   COSM integration, separation of library and script
8 https://github.com/smbaker/pynest/pull/6   Thank you for writing this, I added the feature I was dying to have
```

### Usage list number
`git lpr 6` prints out the URL for 6 so you can use it in [git
cpr](https://github.com/abemassry/git-cpr)

### Output URL (example)
`https://github.com/smbaker/pynest/pull/9`

### In git cpr
`git cpr $(git lpr 6)`
