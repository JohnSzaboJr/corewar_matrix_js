# corewar_matrix_js
Web-based visualisation of corewar, Matrix-style 

![screenshot](https://raw.githubusercontent.com/JohnSzaboJr/corewar_matrix_js/master/screenshot.png)

The javascript reads a js array produced by the virtual machine (written in C), and displays the battle in the "Matrix" style.
Each of the 256 bytes are represented by a character. '\0' is represented by empty space, the rest goes as follows:

1st 63: Japanese katakana

2nd 64: Taiwanese bopomofo

3rd 64: Chinese radicals (Kangxi)

4rd 64: Chinese radicals (Partial)

The characters were selected to give the output a feel similar to one featured in the "Matrix", as Japanese katakana
were used in the movie's visuals as well. The 64-base division was created so that one who is familiar with the characters
can easily identify (at least roughly) the value of each byte.

Additional features:

- Displays the status of the game in a status box "terminal" style
- Pauses on the push of a button
- Up/down arrow keys increase/decrease speed
- Displays basic data of champions
- Displays operation code characters waiting to be executed
- Displays operation names that are currently excuted
- Dosplays cycle number and process number
