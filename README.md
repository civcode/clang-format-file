# my-clang-format-file
Personal .clang-format file for Qt projects.

## How to install clang-format on Ubuntu
```
$ sudo apt-get install clang-format
```
### How to generate basic .clang-format file
```
$ clang-format -style=llvm -dump-config > .clang-format
```
### Where to place .clang-format file
When using with QtCreator place the .clang-format file in src folder or its parent directory. Or place it in the root folder where you store all your code (e.g. /home/$USER/).

### My modifications

- IndentWidth: 4
- AccessModifierOffset: -4
- ColumnLimit: 0   # disable auto line break
- BreakConstructorInitializers: AfterColon
- BreakBeforeBraces: Linux   # [description](https://stackoverflow.com/questions/29477654/how-to-make-clang-format-add-new-line-before-opening-brace-of-a-function)

