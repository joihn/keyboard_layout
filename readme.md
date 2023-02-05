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
for gnome GUI layout selection, add this to `/usr/share/X11/xkb/rules/evdev.xml`

```
    <layout>
      <configItem>
        <name>maximekey</name>
        <!-- Keyboard Custom -->
        <shortDescription>max</shortDescription>
        <description>maximekey</description>
        <languageList>
          <iso639Id>eng</iso639Id>
        </languageList>
      </configItem>
    </layout>
```
![layout](maximekey.png?raw=true "layout")
