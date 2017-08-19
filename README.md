installing
==========
```
gem install kyrbeis
```
using
=====
Create a `~/dotfiles` directory in which your configuration files will be stored.
To add a new configuration file, for example `~/.vimrc`,
create `~/dotiles/__vimrc` in which you will write your vim configuration as usual.

Then, taking care that `~/.vimrc` doesn't already exist (in which case kyrbeis will do nothing),
run:

```
kyrbeis apply
```

Which is just like doing `ln -s ~/dotfiles/__vimrc ~/.vimrc`

Kyrbeis also handles subdirectories, like `~/.config`.
For example, to add a `~/.config/git/ignore`, create `~/dotfiles/__config/git/ignore.`
