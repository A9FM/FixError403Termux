# FixError403Termux
Fix Termux error 403

try:

`apt up -y`

If you get `error 403`, writte this

`termux-setup-storage && curl -o sources.list https://raw.githubusercontent.com/A9FM/FixError403Termux/main/sources.list && cp sources.list $PREFIX/etc/apt/sources.list && rm sources.list && apt up -y`
