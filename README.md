# read_swsh
![License](https://img.shields.io/badge/License-GPLv3-blue.svg)

A script based on kwsch's [pkNX](https://github.com/kwsch/pkNX) project, specifically ported from [Structures/Text/TextFile.cs](https://github.com/kwsch/pkNX/blob/master/pkNX.Structures/Text/TextFile.cs).

read_swsh reads the encoded data from Pokémon games. The script returns table labels, the label's FNV1_64 hash, and the text entry associated with the given files.

![Main Window](https://i.imgur.com/us4FpDl.png)

## Features
Supports:
* Sword and Shield
* Likely Let's Go, Pikachu! / Let's Go, Eevee! as well

Just drag and drop the .tbl and .dat of the specified files onto the script, and it will create a text file with all the decoded data you need!

## Dependencies
This script requires at least Python 3 to run
