
After installing WSL and pip3 `site-packages` folder not on path 
----------------------------------------------------------------

- install WSL - Ubuntu 18.04 
- now I want examples from python package *cheat* to explore linux 
  (but the story would be the same for any package)
- `sudo apt-get update` (because `sudo apt-get install pip3` will not work
   of fresh installation)
- `sudo apt-get install pip3`
- `sudo pip3 install cheat`
- `cheat` not recognised as a command, while `python3` runs fine from
  /usr/bin/python3
- realise `$HOME/.local/lib/python3.6/site-packages` must be on path 
- in `~/.profile` add `$HOME/.local/lib/python3.6/site-packages` to path 
  with `export PATH="$HOME/.local/lib/python3.6/site-packages:PATH"`

#### Links:

- [1](https://unix.stackexchange.com/questions/471783/site-packages-directory-not-found-after-installing-pip3-with-apt-get-in-ubuntu-w)
- [2](https://askubuntu.com/questions/1079021/is-it-possible-to-avoid-setting-path-manually-for-python-package-executables/1079579#1079579)


Why does WSL inherit Windows PATH?
----------------------------------

- https://github.com/Microsoft/WSL/issues/1640


WSL seems to as SSH 
--------------------

```
epo@EP-THINK:/mnt/c/Users/EP/Documents/GitHub/ToDo$ pstree -p
init(1)─┬─init(53)───bash(54)
        ├─init(1688)───bash(1689)───pstree(1699)
        └─sudo(23)───ssh(24)
```

Troubleshooting
---------------

- [corrupt installation](https://github.com/Microsoft/WSL/issues/3352#issuecomment-402673907)
