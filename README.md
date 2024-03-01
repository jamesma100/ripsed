# rsed

Wrapper around sed that allows recursive search. Simply:
```
./rsed -i "s/something/somethingelse/g" ./mydir
```
and it just calls sed on every file under `./mydir`!

Notes:
- must have GNU sed installed; macOS sed will not work - you can get GNU sed on macOS with `brew install gsed`
- need [ripgrep](https://github.com/BurntSushi/ripgrep) installed
- rsed will exclude binary files and hidden files (i.e. files that begin with a `.`) - there is no option to change this currently
