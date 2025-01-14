# groups used with tuckr cmd

------
## zsh

we don't use .zshenv here since it contain per machine tockens and customizations which do not needed to be saved.

Here's the order of execution for Zsh startup files:

1. /etc/zshenv (System-wide)
2. ~/.zshenv (Per-user, always executed)
3. /etc/zprofile (System-wide, login shells)
4. ~/.zprofile (Per-user, login shells)
5. /etc/zshrc (System-wide, interactive shells)
6. ~/.zshrc (Per-user, interactive shells)
7. /etc/zlogin (System-wide, login shells)
8. ~/.zlogin (Per-user, login shells)

On logout:

9. ~/.zlogout
10. /etc/zlogout

Typical usage:
- .zshenv: environment variables, PATH
- .zprofile: login-specific setup
- .zshrc: aliases, functions, prompt, interactive-shell settings


------
