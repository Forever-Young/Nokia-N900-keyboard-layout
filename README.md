Nokia-N900-keyboard-layout
==========================

Hardware keyboard layout for Nokia N900.
For international (UK?) hardware layout, but with additional 2nd layout - Russian.

Installation
------------
1. Backup files:
   - /usr/share/X11/xkb/types/nokia
   - /usr/share/X11/xkb/symbols/nokia_vndr/rx-51
2. Copy corresponding files from this directory to their places
3. In "Text Input" settings - set "English" keyboard
4. For screen keyboard - add second keyboard Russian
5. From xterm - enter "setxkbmap ru_custom"

Usage
-----
To switch layout - press Shift-Space

Changes
-------
1. Changed eurosign and sterling to []
2. Changed many Fn-SH combinations: digits to F1-F10, letters
3. Tab, ESC, Menu
4. Fn+Cursor - Home/End/PgUp/PgDn
5. For russian layout - combined Left/Up, Right/Down
6. For russian layout - letters on the same place as on Russian hardware variant
7. For russian layout - fixed capital hardsign, yu

Layout (English)
----------------
<pre>
|-------+----+----+----+----+----+----+----+----+----+----+----+-----|
| Fn+SH | F1 | F2 | F3 | F4 | F5 | F6 | F7 | F8 | F9 | F10| F11| F12 |
| Fn    | 1  | 2  | 3  | 4  | 5  | 6  | 7  | 8  | 9  | 0  | =  | Tab |
| SHIFT | Q  | W  | E  | R  | T  | Y  | U  | I  | O  | P  | ;  | Del |
|       | q  | w  | e  | r  | t  | y  | u  | i  | o  | p  | ,  | BKSP|
|-------+----+----+----+----+----+----+----+----+----+----+----+-----|
| Fn+SH | *  | +  | #  | -  | _  | ~  | {  | }  | !  | |  |    | MENU|
| Fn    | *  | +  | #  | -  | _  | (  | )  | &  | !  | ?  |PgUp| ESC |
| SHIFT | A  | S  | D  | F  | G  | H  | J  | K  | L  | :  |    | RET |
|       | a  | s  | d  | f  | g  | h  | j  | k  | l  | .  | Up | RET |
|-------+----+----+----+----+----+----+----+----+----+----+----+-----|
| Fn+SH |none|none| ^  | <  | >  | %  | `  |   @     |    |    |     |
| Fn    | [  | $  | ]  | /  | \  | "  | '  |   @     |Home|PgDn| End |
| SHIFT | Z  | X  | C  | V  | B  | N  | M  | Layout  |    |    |     |
|       | z  | x  | c  | v  | b  | n  | m  |   SPC   |Left|Down|Right|
|-------+----+----+----+----+----+----+----+---------+----+----+-----|
</pre>

TODO
----
1. Fix Fn-SH-h - dead_tilde
2. Something for Fn-SH-a, s, d, f, g, l?
3. Keyboard layout applet for status-menu
4. Same marks for Russian layout

Credits
-------
Some part of layout is taken from https://github.com/vahit/N900-HKlayout
