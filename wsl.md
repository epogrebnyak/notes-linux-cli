From DOS to Linux
=================

Windows Subsytem for Linux (WSL)
--------------------------------

- [install guide](https://msdn.microsoft.com/en-us/commandline/wsl/install_guide)
- WSL is a great way to have working Linux shell on Windows, 
  [read more here](https://docs.microsoft.com/en-us/windows/wsl/about)
- `wsl | ubuntu | bash` - use either to call WSL
- [wslconfig.exe](https://docs.microsoft.com/en-us/windows/wsl/wsl-config)
  helps configuring multiple linux distrubutions on Windows
  

Terminals 
---------

- my usual terminal is [cmder](http://cmder.net)
- [hyper](https://hyper.is) seems a nicely colored terminal
- reading about [terminology](https://unix.stackexchange.com/questions/4126/what-is-the-exact-difference-between-a-terminal-a-shell-a-tty-and-a-con)

Prompt
------

- prompt is whatever shell types for you as a welcome message
- `echo $PS1` shows your prompt configuration
- you can change the prompt by setting `$PS1` with `export`:
  - bare minimum `export PS1="$ "` 
  - time, date, current folder, newline and `$` `export PS1="\D{%Y-%m-%d} \A \w\n\$ "`
- `~/.bashrc` file holds your default `$PS1` configuarion, `. ~/.bashrc` reloads this 
  configuration

#### Links:

- [explore prompt configuration](http://bashrcgenerator.com)
- https://bneijt.nl/blog/post/add-a-timestamp-to-your-bash-prompt/
- https://askubuntu.com/questions/372849/what-does-debian-chrootdebian-chroot-do-in-my-terminal-prompt

Get better advice: cheat and cheat.sh
-------------------------------------

- `man` is complete, but lengthy and notorious to read
- `cheat` and `cheat.sh` are nifty

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

- https://unix.stackexchange.com/questions/471783/site-packages-directory-not-found-after-installing-pip3-with-apt-get-in-ubuntu-w
- https://askubuntu.com/questions/1079021/is-it-possible-to-avoid-setting-path-manually-for-python-package-executables/1079579#1079579


Why does WSL inherit Windows PATH?
----------------------------------

- https://github.com/Microsoft/WSL/issues/1640


WSL seems to run ssh 
--------------------

```
epo@EP-THINK:/mnt/c/Users/EP/Documents/GitHub/ToDo$ pstree -p
init(1)─┬─init(53)───bash(54)
        ├─init(1688)───bash(1689)───pstree(1699)
        └─sudo(23)───ssh(24)
```




