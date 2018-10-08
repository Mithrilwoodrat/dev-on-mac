# dev-on-mac
An opiniated guide to set up a development environment on Windows.


## Setup bash completion
<https://stackoverflow.com/questions/12399002/how-to-configure-git-bash-command-line-completion>

Homebrew
if $BASH_VERSION > 3: `brew install bash-completion@2` (updated version)

add to .bash_profile:
```
  if [ -f /usr/local/share/bash-completion/bash_completion ]; then
    . /usr/local/share/bash-completion/bash_completion
  fi
```
For older versions of bash: `brew install bash-completion`

add to .bash_profile:

```
[ -f /usr/local/etc/bash_completion ] && . /usr/local/etc/bash_completion
```
