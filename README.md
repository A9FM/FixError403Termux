# FixErrorTermux
Fix Termux error

try:
```
pkg update && pkg upgrade -y
```

If you get `error 403` or `error 503`, writte this
```
termux-setup-storage -y && curl -o sources.list https://raw.githubusercontent.com/A9FM/FixError403Termux/main/sources.list && rm -rf $PREFIX/etc/apt/sources.list.d/ && cp sources.list $PREFIX/etc/apt/sources.list && rm sources.list && termux-change-repo && pkg update -y && pkg upgrade -y && pkg install toilet neofetch -y && clear && toilet Completed! && neofetch
```
Or install → <a href="https://f-droid.org/repo/com.termux_118.apk">Termux 0.118</a> ←


