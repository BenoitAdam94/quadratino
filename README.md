# quadratino
A (shitty) Snake clone for GameBoy written in C with gbdk. This should a decent start point to code something with gbdk.

Take a look at [awesome-gbdev](https://github.com/avivace/awesome-gbdev), a curated list of awesome GameBoy Development resources, tools, docs, related projects and open-source ROMs. 

Compile with gbdk

`bin\lcc -Wa-l -Wl-m -Wl-j -DUSE_SFR_FOR_REG -c -o  quadratino.o  quadratino.c
bin\lcc -Wa-l -Wl-m -Wl-j -DUSE_SFR_FOR_REG -o  quadratino.gb  quadratino.o`

or download the [ready ROM](https://github.com/avivace/quadratino/raw/master/quadratino.gb) (may not be the latest build)

Reccomended emulator: [bgb](http://bgb.bircd.org/)



Changes (06/07/2019)

- mode=1;" at line 63 (removed)
- RAND defined to UINT8
- n defined a bit before
- change rand.h to <gb/rand.h>
- added res.h instead of including C (remove "Multiple definition of _tail_tile_data" when compiling with the new "Make")

- added make for Win+Linux (by flozz)
