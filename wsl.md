Windows Subsytem for Linux (WSL)
--------------------------------

- `wsl | ubuntu | bash` - use either to call WSL
- [wslconfig.exe](https://docs.microsoft.com/en-us/windows/wsl/wsl-config)
  helps configuring multiple linux distrubutions on Windows
- [install guide](https://msdn.microsoft.com/en-us/commandline/wsl/install_guide)
- after you log in run `sudo apt-get update` to refresh packages


[Terminals][so-terminology]
----------------------------

- my usual terminal is [cmder](http://cmder.net)
- [hyper](https://hyper.is) seems a nicely colored terminal, but has few errors
- Windows Terminal is coming, but unclear for me how to install

[so-terminology]: https://unix.stackexchange.com/questions/4126/what-is-the-exact-difference-between-a-terminal-a-shell-a-tty-and-a-con

Prompt
------

- prompt is whatever shell types for you as a welcome message
- `echo $PS1` shows your prompt configuration
- you can change the prompt by setting `$PS1` with `export`:
  - bare minimum `export PS1="$ "` 
  - time, date, current folder, newline and `$` `export PS1="\D{%Y-%m-%d} \A \w\n\$ "`
- `~/.bashrc` file holds your default `$PS1` configuarion, `. ~/.bashrc` reloads this 
  configuration

Get better advice: cheat and cheat.sh
-------------------------------------

- `man` is complete, but lengthy and notorious to read
- `cheat` and `cheat.sh` are nifty
