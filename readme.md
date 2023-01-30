A custom keyboard layout optimized for code and french language, inspired by Eurkey and CH layout. No dead key.
Put `maximekey` in `/usr/share/X11/xkb/symbols`
then 
`
setxkbmap maximekey -option && setxkbmap maximekey -option lv3:lsgt_switch -option caps:escape
`


alias to activate selectively swiss layout or maximekeys layout
```
alias ch="setxkbmap ch -variant fr -option && setxkbmap ch -variant fr -option caps:escape"
alias eur="setxkbmap maximekey -option && setxkbmap maximekey -option lv3:lsgt_switch -option caps:escape"
```

![layout](maximekey.png?raw=true "layout")
