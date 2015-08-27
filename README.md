# Arduino + OSX + C++11 + Make Boilerplate

This repro is a boilerplate template for starting new arduino projects
on osx.  It could probably be easily adapted to other osx by modifying the
Makefile paths appropriately.

## Installation

1. Clone the repro
2. `git submodule init`
3. `git submodule update`
4. `brew install avr-libc` (or use macports)

## Using

1. Write your code in a combination of .cpp/.h files, by convention, the main
   file should be end with .ino
2. Add names of any necessary libraries into the libraries.mk file
3. Edit board.mk to set the board to the appropriate board.  
4. `make` to build
5. `make upload` to upload via avrdude
6. `make monitor` to connect to the serial point.
7. To Exit the monitor, press `ctrl-a, k, y`


# Contributing

If you find a bug that you fix, or decide to help support other oses, please
feel free to submit pull requests.  Make sure you add your name to the
CONTRIBUTERS.md file
