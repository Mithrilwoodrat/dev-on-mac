# dev-on-mac
An opiniated guide to set up a development environment on Mac.

## Setup zsh(Optional)
<https://sourabhbajaj.com/mac-setup/iTerm/zsh.html>

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

## Setup bash git completion

```
curl https://raw.githubusercontent.com/git/git/master/contrib/completion/git-completion.bash -o ~/.git-completion
```

add 
```
if [ -f ~/.git-completion ]; then
  . ~/.git-completion
fi
```
to ~/.bashrc

## Setup MySQL
`brew install mysql@5.6`
`echo 'export PATH="/usr/local/opt/mysql@5.6/bin:$PATH"' >> ~/.zshrc`
`brew services start mysql@5.6`

Using `mysqladmin -u root password 'yourpassword' ` to set root password

<https://gist.github.com/nrollr/3f57fc15ded7dddddcc4e82fe137b58e>

## Setup Docker

Download from https://store.docker.com/editions/community/docker-ce-desktop-mac
