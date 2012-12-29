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
5. In xterm - type "setxkbmap ru_custom" - to try
6. For permanent - type "gconftool-2 -s -t string /apps/osso/inputmethod/int_kb_layout ru_custom"

Usage
-----
To switch layout - press Shift-Space

Changes
-------
1. Changed eurosign and sterling to []
2. Changed many Fn-SH combinations: digits to F1-F10, letters
3. Tab, ESC, Menu, Delete
4. Fn+Cursor - Home/End/PgUp/PgDn
5. For russian layout
   - combined Left/Up, Right/Down
   - letters on the same place as on Russian layout
   - fixed capital hardsign, yu
   - period and comma - Fn+Up, Shift+Fn+Up
   - question and colon - Fn+LatComma, Shift+Fn+LatComma

Layout (English)
----------------
<pre>
|-------+----+----+----+----+----+----+----+----+----+----+----+-----|
| Fn+SH | F1 | F2 | F3 | F4 | F5 | F6 | F7 | F8 | F9 | F10| F11| F12 |
| Fn    | 1  | 2  | 3  | 4  | 5  | 6  | 7  | 8  | 9  | 0  | =  | Del |
| SHIFT | Q  | W  | E  | R  | T  | Y  | U  | I  | O  | P  | ;  | Tab |
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

Layout (Russian)
----------------
<pre>
|-------+----+----+----+----+----+----+----+----+----+----+----+-----|
| Fn+SH | F1 | F2 | F3 | F4 | F5 | F6 | F7 | F8 | F9 | F10| Ъ  | F12 |
| Fn    | 1  | 2  | 3  | 4  | 5  | 6  | 7  | 8  | 9  | 0  | ъ  | Del |
| SHIFT | Й  | Ц  | У  | К  | Е  | Н  | Г  | Г  | Ш  | З  | Х  | Tab |
|       | й  | ц  | у  | к  | е  | н  | г  | г  | ш  | з  | х  | BKSP|
|-------+----+----+----+----+----+----+----+----+----+----+----+-----|
| Fn+SH | *  | +  | #  | -  | _  | ~  | {  | }  | !  | :  | ,  | MENU|
| Fn    | *  | +  | #  | -  | _  | (  | )  | &  | !  | ?  | .  | ESC |
| SHIFT | Ф  | Ы  | В  | А  | П  | Р  | О  | Л  | Ж  | Ж  | Э  | RET |
|       | ф  | ы  | в  | а  | п  | р  | о  | л  | д  | ж  | э  | RET |
|-------+----+----+----+----+----+----+----+----+----+----+----+-----|
| Fn+SH |none|none| ^  | <  | >  | %  | `  |   @     | Ю  |    |     |
| Fn    | [  | $  | ]  | /  | \  | "  | '  |   @     | ю  | Up | Down|
| SHIFT | Я  | Ч  | С  | М  | И  | Т  | Ь  | Layout  | Б  |    |     |
|       | я  | ч  | с  | м  | и  | т  | ь  |   SPC   | б  |Left|Right|
|-------+----+----+----+----+----+----+----+---------+----+----+-----|
</pre>

TODO
----
1. Something for Fn-SH-a, s, d, f, g, l?
2. Keyboard layout applet for status-menu

Credits
-------
Some part of layout is taken from https://github.com/vahit/N900-HKlayout
