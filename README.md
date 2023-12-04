# ghostbusters
Remake of Activision's 1984 Ghostbusters game

This is a remake of David Crane's awsome Ghostbusters game as first released by Activision on the C64. The game requires the 32k memory expansion and can be burned to a 512k banking cartridge that uses the non-inverted banking method or can run from a FinalGrom or similar flashcart that can support images of 512kb and larger (the BackBit might work).
The game is a complete remake, not a port from existing source code or dissassembly efforts. Although I tried to make it feel as much as the C64 original as possible, there might be small differences in how it plays. Most of the graphics are inspired by the Sega Master System version of the game, but several parts have been re-created from scratch.

## Building the game

In order to build the game, you'll need a copy of the gcc compiler for the tms9900 CPU which can be found [here](https://github.com/mburkley/tms9900-gcc). The Makefiles expect the gcc binaries to be in your path. Furthermore, the build system includes some bash scripts which have been tested on Linux and macos, building on Windows will require jumping through some hoops, I'm afraid. WSL might work.
If the above pre-requisites are fulfilled, you can simple issue a `make` command which will build ghostbusters.bin (rename to ghostbusters8.bin to use in Classic99, or use as-is in js99er.net and BulWHiP) and ghostbuster.rpk (for use in Mame and js99er.net).
