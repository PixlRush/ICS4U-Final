# ICS4U1-E1 Final Project
## Proposal
I would like to make a game of minesweeper. The game will have multiple difficulty levels and will be controlled by a command-line input. This will show recursion through its dig method which if it finds nothing will dig everywhere around itself. It will use an array of objects as its board. The object base will be the super class to many children classes under it (mine, flag, etc...). This will also include special modes that vary their digging styles and notation. It will hold the 5 fastest times in a file for your difficulty and style.
## UML
### Minesweeper
```
Board field
```
```
public static void main(String[] args)
```
### Board
```
Tile[][] field
int len
int wid
int mine
int digStyle
```
```
cmd()
boolean dig(x,y)
void flag(x,y)
```
### Tile
```
int surround
int style
boolean dug
boolean flagged
```
```
boolean dig(style)
int search(style)
flag()
boolean getDug()
boolean getFlagged()
```
### `Tile >` Mine
```
boolean detonated
```
### `Tile >` Blank
## Test Cases
