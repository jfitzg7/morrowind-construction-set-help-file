# TES III: Morrowind Construction Set Help File Conversion
The Elder Scrolls III: Morrowind was released in 2002, and this means that some of the files (such as the Construction Set's help file) included with the game are deprecated. Bethesda games are well known for being modder-friendly since they release their development tools along with their games. In Morrowind, the development tool is called the Construction Set and it is typically included in the installation of the game. However, the Steam version of Morrowind does not currently provide the Construction Set. For Steam users, the Morrowind Construction Set can be downloaded [here on NexusMods](https://www.nexusmods.com/morrowind/mods/42196). The documentation for the Construction Set from NexusMods is in the WinHelp (`.hlp`) format, which cannot be opened on Windows 10 or 11. This repo is intended to store conversions of the original Construction Set help file that can be viewed on modern Windows operating systems.

## helpdeco ([GitHub Link](https://github.com/pmachapman/helpdeco))
The `helpdeco` utility can be used to decompile `.hlp` files into their core components, which can then be reconstructed into other file formats such as `.chm`. This tool was used to convert the original Construction Set `.hlp` file into an `.rtf` (Rich Text Format) file, which can be viewed on modern Windows versions in applications such as WordPad. Although this tool got most of the job done, it was not able to include the last few paragraphs of the original help file, and the images needed to be included manually. An alternative to `helpdeco` is [this website](https://ehubsoft.herokuapp.com/chmviewer/), which actually does capture everything and includes all of the images.

## TODO
* Look into generating alternative file formats (such as `.chm`)
* Understand why `helpdeco` has troubles generating the `.rtf` correctly
* Manually add in the remaining text to the `.rtf` file
