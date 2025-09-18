## Building from source

To build Luma3DS, the following is needed:
* git
* [makerom](https://github.com/jakcron/Project_CTR) in `$PATH`
* [firmtool](https://github.com/TuxSH/firmtool) installed
* up-to-date devkitARM and libctru:
    * install `dkp-pacman` (or, for distributions that already provide pacman, add repositories): https://devkitpro.org/wiki/devkitPro_pacman
    * install packages from `3ds-dev` metapackage: `sudo dkp-pacman -S 3ds-dev --needed`
    * while libctru and Luma3DS releases are kept in sync, you may have to build libctru from source for non-release Luma3DS commits

While Luma3DS releases are bundled with `3ds-hbmenu`, Luma3DS actually compiles into one single file: `boot.firm`. Just copy it over to the root of your SD card ([ftpd](https://github.com/mtheall/ftpd) is the easiest way to do so), and you're done.

## Licensing
This software is licensed under the terms of the GPLv3. You can find a copy of the license in the LICENSE.txt file.

Files in the GDB stub are instead triple-licensed as MIT or "GPLv2 or any later version", in which case it's specified in the file header. PM, SM, PXI reimplementations are also licensed under MIT.

## Credits

Luma3DS would not be what it is without the contributions and constructive feedback of many. We would like to thanks in particular:

* **[@devkitPro](https://github.com/devkitPro)** (especially **[@fincs](https://github.com/fincs)**, **[@WinterMute](https://github.com/WinterMute)** and **[@mtheall](https://github.com/mtheall)**) for providing quality and easy-to-use toolchains with bleeding-edge GCC, and for their continued technical advice
* **[@Nanquitas](https://github.com/Nanquitas)** for the initial version of the game plugin loader code as well as very useful contributions to the GDB stub
* **[@piepie62](https://github.com/piepie62)** for the current implementation of the Rosalina cheat engine, **Duckbill** for its original implementation
* **[@panicbit](https://github.com/panicbit)** for the original implementation of screen filters in Rosalina
* **[@jasondellaluce](https://github.com/jasondellaluce)** for LayeredFS
* **[@LiquidFenrir](https://github.com/LiquidFenrir)** for the memory viewer inside Rosalina's "Process List"
* **ChaN** for [FatFs](http://elm-chan.org/fsw/ff/00index_e.html)
* Everyone who has contributed to the Luma3DS repository
* Everyone who has assisted with troubleshooting end-users
* Everyone who has provided constructive feedback to Luma3DS
