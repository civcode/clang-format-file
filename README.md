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
- ColumnLimit: 90

## How to set up QtCreator 
(clang-format must be installed on your system)
- activate beautifier plugin (help > about plugins > Beautifier)
- enable auto format (tools > options > Beautifier > General > Enable auto format on file save)
- select ClangFormat (tools > options > Beautifier > General > Tool: "ClangFormat") 
- select File (tools > options > Beautifier > Clang Format > Options > Use predefined style: "File")
  - (you don't set a file path here. clang-format looks for the .clang-format file as described above)


