## Keyboard shortcuts

Note that window in Emacs is the physical area of the screen in which a buffer is displayed. These shortcuts won't work if you have bound them to do other commands.


### Buffer Commands

#### Move inside buffer

| Shortcut    | Description                          |
|-------------|--------------------------------------|
| C-M-n       | Move cursor to next maching bracket  |
| C-M-a       | Move to begining of function         |
| C-M-e       | Move cursor to end of function       |
| C-e         | Move cursor to end of line           |
| C-n         | Move cursor to next line             |
| M-<         | Move cursor to start of buffer       |
| M->         | Move cursor to end of buffer         |
| C-x-o       | Move cursor to next buffer           |
| C-u C-Space | Goto last cursor point within buffer |


#### Selection inside buffer

| Shortcut | Description                                         |
|----------|-----------------------------------------------------|
| C-M-h    | Select current function                             |
| C-x-h    | Select whole buffer                                 |
| C-Space  | Start selection (Now move the cursor to select text |


#### More buffer commands

| Shortcut    | Description                                                  |
|-------------|--------------------------------------------------------------|
| C-x-0       | Close current buffer                                         |
| C-x-b-Tab   | Display list of all buffers                                  |
| C-x-b       | Move to any of previous buffers given name                   |
| C-x C-Space | Goto last cursor point (it can jump across multiple buffers) |

### Text Commands

| Shortcut     | Description                    |
|--------------|--------------------------------|
| C-k          | Cut text in current line       |
| C-Shift-BKSP | Cut current line               |
| M-c          | Change next word to camel case |
| M-u          | Change next word to upper case |
| M-q          | Break line to paragraph at point|

## Emacs Org Mode Table Commands

| Shortcut  | Description                                         |
|-----------|-----------------------------------------------------|
| C-c ?     | Find reference of particular field                  |
| C-u C-c * | Recalculate all forumlas inside current spreadsheet |
| C-c {     | Turn on the formula debugger                        |
| C-c }     | Turn on table reference visualization grid          |
| C-c C-c   | Evaluate formula at current field                   |
| C-c =     | Edit formula at current field                       |

## List Of Org Mode Table Formula Functions
| Name             | Function                     |
|------------------|------------------------------|
| vmean            | Find mean of range of values |
| vsum             | Find sum of values           |
| substring        |                              |
| number-to-string |                              |
| round            |                              |



## Useful Commands

Break long line to single line at cursor point
```
    fill-paragraph
```
Break region into single line
```
    fill-region
```
Delete column of values
```
    kill-rectangle
```

## Emacs Org Mode Tables
Index first row of table
```
    @1
```
Index first column of table
```
    $1
```
Index first field of table
```
    @1$1
```
Example of column formula
```
    $3 = $1+$2
    $3 = @1$1+@1$2
```
Be careful about the last one.  
Example of field formula
```
    @1$3 = @1$1+@1$2
```
Format of table formula below table
```
#+TBLFM: formula1 :: formula2 :: formula3
```
Reference remote table `members` in another table values
```
    #+TBLNAME: members
    | Peter|10|

    #+TBLNAME: values
    |Value |10 |
    #+TBLFM: @1@2=remote(members,@1@2)
```
Calculate sum of column from row `@1` to `@12` of column `$1`.
```
    :=vsum(@1$1..@12$1)
```


### Points
1. Two types of formulas - column formulas and field formulas.
2. Column formulas applies ot every row of that column.
3. Formula starts with `#+TBLFM:`. Each forumla is seperated by `::`.

## Keyboard Macros
Keyboard Macros can be used to record sequence of key actions.
### How to define keyboard macro
Start defining keyboard macro
```
    C-x (
```
Stop defining keyboard macro
```
    C-x )
```
Execute keyboard macro on current line
```
    C-x e
```
Execute keybaord macro 4 times
```
    C-u 4 C-x e
```

## GDB Commands
Split screen into multiple windows showing different buffers related to debugging
```
    gdb-many-windows
```


## Artist Mode
To start artist mode
```
    artist-mode
```
Draw rectangle
```
    artist-select-op-rectangle
```


## References
[ColumnFormula](http://orgmode.org/manual/Column-formulas.html)
