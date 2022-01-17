# FixError403Termux
Fix Termux error 403

try:

`apt up -y`

If you get `error 403`, writte this

`termux-setup-storage -y && curl -o sources.list https://raw.githubusercontent.com/A9FM/FixError403Termux/main/sources.list && rm -rf $PREFIX/etc/apt/sources.list.d/ && cp sources.list $PREFIX/etc/apt/sources.list && rm sources.list && termux-change-repo && pkg update && pkg upgrade -y && pkg install toilet -y && clear && toilet Completed!`
