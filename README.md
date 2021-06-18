# read_swsh
![License](https://img.shields.io/badge/License-GPLv3-blue.svg)

A script based on kwsch's [pkNX](https://github.com/kwsch/pkNX) project, specifically ported from [Structures/Text/TextFile.cs](https://github.com/kwsch/pkNX/blob/master/pkNX.Structures/Text/TextFile.cs).

read_swsh reads the encoded data from gen 8 Pokémon games. The script returns the table's labels, the label's FNV1_64 hash, and the label's flavor text.

More information about what goes on in the background can be found [here](https://projectpokemon.org/home/forums/topic/48656-lgpe-romfs-data-reverse-engineering/).

Example file output from Pokémon Sword's zukan_comment_A table:
![Main Window](https://i.imgur.com/Uz621uL.png)

## Features
Supports:
* Pokémon Sword 
* Pokémon Shield
* Pokémon Let's Go, Pikachu!
* Pokémon Let's Go, Eevee!

You will need the supported game's .dat and .tbl files, which are found in their decompressed RomFS.

The files will be found in the RomFS directory: bin > message > language > common

Do note that not all of the flatbuffer delimiters and variables are supported, so some of the table entries will have garbage output.

This script mostly focuses on the zukan_comment_A and zukan_comment_B tables, but some of the other tables will also decompress just fine.

## Dependencies
This script requires at least Python 3 to run
