# Colecrux

This is an XKB layout for Colecrux. 

Colecrux starts with Colemak DH with the Angle and Wide mods.
- Angle shifts the bottom left keys so your left hand can rotate a bit clockwise.
- Wide shifts the right hand block right one key.
- DH, also known as Curl, moves D and H down, along with G.

See [Dreymar's Big Bag of Tricks, Ergonomy section](https://dreymar.colemak.org/ergo-mods.html)


Then french accented letters are added as a layer on AltGr.  No dead keys.

![Colemak DH Angle Wide](Colemak%20DH%20Angle%20Wide%20Layout.png)
![Colemak DH Angle Wide Shift layer](Colemak DH Angle Wide Shift Layout.png)
![Colemak DH Angle Wide AltGr layer](Colecrux AltGr layer.png)


## Installing

Add `symbols_us_colecrux` to `/usr/share/X11/xkb/symbols/us`.

Add this block in both `/user/share/X11/xkb/rules/base.xml`and `evdev.xml`.

```
        <variant>
          <configItem>
            <name>colecrux</name>
            <description>English (Colecrux)</description>
          </configItem>
        </variant>
```

At least log-off then log-on is required for the changes to take effect.

