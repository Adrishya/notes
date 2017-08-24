# VIM

* You enter command from command-mode.
* Settings of vim are stored in `.vim` file.
* You can have different bindings in 
* 3 modes in vim - command mode, insert mode, replace mode.
* hkjl - arrow keys for vi.
* Shortcuts for Window start with `Ctrl+w`.
* `sp` is short for split.
* You can append a number (seperated by space) before most of the commands.

# Basic Shortcuts
| Shortcut | Explanation                                    |
|----------|------------------------------------------------|
| c        | Command mode - this is the mode vim open with  |
| i        | Insert mode - enter this mode to edit the file |
| u        | Undo                                           |
| Ctrl+r   | Redo                                           |
| /        |                                                |
| gg       | Goto top most point in file                    |
| Shift    |                                                |
| $        | End of line                                    |
| End      | Endi of line                                   |
| Home     | Start of line                                  |
| 0        | Start of line                                  |
| ^        | Start of first word in line                    |
| b        | Move from one word to another backwards        |
| w        | Move from one word to another forwards         |
| x        | Delete                                         |
| dd       | Delete current line                            |
| .        | Execute previous command                       |


# Window shortcuts
| Shortcut         | Explanation                                       |
|------------------|---------------------------------------------------|
| Ctrl+w+o         | Close all windows leaving the current window open |
| Ctrl+w+Arrow key | Move between windows                              |
| Ctrl+w+s         | Split window horizontally                         |
| Ctrl+w+v         | Split window vertically                           |

# Commands
| Shortcut | Explanation               |
|----------|---------------------------|
| sp       | Split window horizontally |
| vsp      | Split vertical vertically |


## Visual block
* Visual is used for wide variety of selections and then performing operations on the selection.

### Commands
| Shortcut | Explanation                                                                                                      |
|----------|------------------------------------------------------------------------------------------------------------------|
| Ctrl+v   | Select block of text starting with selection of zero characters - you can move around to select text.            |
| Shift +v | Select block of text starting with selection of current line - you can move up or down to select line more lines |

* Smallest unit of selection in `Shift+v` is line. 
* Smallest unit of selection in `Ctr+v` is character.

