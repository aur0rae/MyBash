## About
This is my repo where I host my custom shell prompts for use on my Linux systems. It includes a set of aliases for compatibility with some of the command line tools I like and adds some visual flare to my terminal.

<img src="https://github.com/aurorae-nb/bash-customizations/blob/main/res/bash.png">

## Installation
Move your config of choice to `~/.bashrc` and either reload the config or restart your terminal emulator. If you do not want to use any of the below tools or they are not shipped by your distro, you may opt to instead remove them from your config file by deleting any `alias`es or other commands referencing them. For this to work by default though, you will need the following:
- `bat`/`batcat`
- `zoxide`
- `fzf`
- `eza`
- `git`
```sh
mv ./bash-[profile] ~/.bashrc
source .bashrc
```

If the `git` integration breaks, find where `git-prompt.sh` is on your system and the config accordingly. On Arch systems, it's located at `/usr/share/git/git-prompt.sh`, so this is what I have it default to. Various forms of `locate` or simply the `find` command can be helpful to figure out where it is. If you want to use the Nordic theme, also install [Starship](https://starship.rs/)
```sh
sudo find / -name git-prompt.sh
curl -sS https://starship.rs/install.sh | sh
```

## Credits
Thanks to the couple people on the StyroPyro Discord server that helped me figure out how to do this! Secondarily, `starship.toml` is borrowed from Chris Titus' [Beautiful Bash](https://github.com/christitustech/mybash).
