# Colecrux

This is the ColeCrux keyboard layout project.  It has a XKB layout and a Windows layout. 

Colecrux starts with Colemak DH with the Angle and Wide mods.
- Angle shifts the bottom left keys so your left hand can rotate a bit clockwise.
- Wide shifts the right hand block right one key.
- DH, also known as Curl, moves D and H down, along with G.

See [DreymaR's Big Bag of Tricks, Ergonomy section](https://dreymar.colemak.org/ergo-mods.html)

Then french accented letters are added as a layer on AltGr.


#### Colemak DH Angle Wide
![Colemak DH Angle Wide](Colemak%20DH%20Angle%20Wide%20Layout.png)

#### Colemak DH Angle Wide, shift layer
![Colemak DH Angle Wide Shift layer](Colemak%20DH%20Angle%20Wide%20Shift%20Layout.png)

#### Colecrux AltGr layer
![ColeCrux AltGr layer](Colecrux%20AltGr%20layer.png)

#### Colecrux AltGr+Shift layer
![ColeCrux AltGr+Shift layer](Colecrux%20AltGr+Shift%20layer.png)


## Installing

### Linux

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


### Windows

Use Microsoft Keyboard Layout Creator to load `ColeCrux.klc`.  Then use the "Build DLL and
Setup Package" command.  The resulting installer can then be used to install the layout.

After installation, a sign-off/sign-in is needed to get the "ColeCrux" name in the keyboard tray icon.

Before installing a new version of the keyboard, use the old installer to remove the current keyboard.  
It might be better even to then sign-off/in before building and installing the new.  Which then requires
another sign-off/in to be sure all the Windows software is up to date.

Microsoft Keyboard Layout Creator 1.4 has an issue with the description field in Properties.  It may
show a value by another one will actually be used.  Create your layout, then save the KLC file.
Use a text editor and make sure the description is correct before building.


### Attribution

The image of the Colemak CurlAWide layouts were taken from [DreymaR's EPKL software](https://github.com/DreymaR/BigBagKbdTrixPKL).


## Future

Add symbols:
- ✓, check mark, U+2713
- ✗, ballot X, U+2717


## Development notes

### French

- à: U+00E0
- è: U+00E8
- ù: U+00F9
- é: U+00E9
- â: U+00E2
- ê: U+00EA
- î: U+00EE
- ô: U+00F4
- û: U+00FB
- ä: U+00E4
- ë: U+00EB
- ï: U+00EF
- ç: U+00E7
- «: U+00AB
- »: U+00BB


### Misc

- 38°: degree, U+00B0
- →: right arrow, U+2192
- ←: left arrow, U+2190
- ↑: upward arrow, U+2191
- ↓: downward arrow, U+2193
- ↔: horizontal arrow, both ways, U+2194


### Mathematics

- ×: multiplication, U+00D7
- ÷: division, U+00f7
- x²: power of 2, U+00B2
- x³: power of 3, U+00B3
- ±: plus or minus, U+00B1
- ≤: less than or equal: U+2264
- ≥: greater than or equal: U+2265
- ≈: approximately equal, U+2248
- √: square root, U+221A
- ∑: summation: U+2211


### Greek

- π: pi, U+03C0
- μ: mu, U+03BC
- Δ: capital delta
