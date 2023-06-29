# Bash PS1 Code

## PS1:

![ps1 image](image.png)

## Copy this code to .bashrc

```
git_branch() {
  git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/(\1)/'
}
export PS1="\[\e[0;31m\]\u\[\e[m\]@\[\e[0;94m\]\h\[\e[m\]: \[\e[0;32m\]\W\[\e[m\] 🦈\[\e[0;91m\]\$(git_branch)\[\e[m\]\[\e[0;36m\]> \[\e[m\]"
```
