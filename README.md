
## Vim tutorial

### Modes
Vim has three different modes: 
* **Insert mode:** You write text as in any text editor.
* **Normal mode:** Normal mode provides you efficient ways to manipulate text.
* **Visual mode:** Not commonly used.

At any time you can see which mode you are in by looking in the left-bottom corner of the terminal.

To change between modes, use the **Escape key** to enter normal mode, and the **i** key to enter Insert mode.

### Navigation
In contrast to a regular text editor, you can use the keys: **h** (left), **j** (down), **k** (up), and **l** (right) to instead of the arrow keys to move around the text. Note: This only works in **normal mode**. It might be confusing at first, but soon enough it will come natural to you.

To navigate text in terms of words, you can use the keys **w**, **b**, and **e**:

| Key  | Result  |
|---|---|
| w | Move to the start of next word  |
| e | Move to the end of current/previous word  |
| b | Move to the beginning of current/previous word  |

Moving in the text is not limited to individual keys. You can combine movement with a **number**. For example, **5h** is the same as pressing the **h**-key 5 times.

Use **0** to reach the beginning of a sentence and **$** to reach the end of a sentence.

**gg** takes you to the beginning of the file and **G** to the end.

To jump to a specific like, combine a number with the **G**-key, e.g. **3G**.

### Insertion

You can also insert text multiple times. For example, an underline of a header might consists of 30 **-**. Typing  **30i-** and then pressing the **Escape**-key will results in 30 iterations of typing the **-** character. 

Use **o** insert a new line below current line and **O** to insert a line above the current line. After the action, Vim will automatically go into **insert mode**.

Use **x** to delete the current character and **X** to delete the character to the left.

Replace: When you need to replace just one character at the current cursor position, use **r** followed by the character you wish to add.

Delete: **d** is the delete command. You can combine it with numbers and movements. For example, **dw** deletes the first word on the right side, and **3dw** deletes the three coming words to the right side. It also copies the deleted word(s), which can be pasted again using the **p**-key.

Repetition: To repeat the last action, use the **.**-key. 

### Search and Find

To find and move to the next or previous occurrence of a character, use **f** and **F**. Example: **fo** finds next the **o** character.

You can combine **f** with a number. In this example you find the fifth occurrence of **o** by typing: **3fo**.

Based on your cursor position (which word it is currently under), you can jump to the next and previous occurrence of that word by pressing the __*__-key (next) or the **#**-key (previous). 

Searching text is a vital part of any text editor. In Vim you type **/** (shift + 7) along with the text you are searching for. You can continue the search by going to the next (**n**) or previous (**N**) occurrence of the word.

### Jumping

Text structured with parenthesis **(** or brackets **{** or **[** allows you to jump to the matching parenthesis or bracket by clicking **%** (shift + 5). This allows programmers to easily navigate to the end of a function.
