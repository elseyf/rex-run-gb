# rex-run-gb
Game Boy port of the Rex Run Game from Chrome \
This is a (mostly) faithful port of the Game, considering the limitations of the Game Boy

In order to build the rom, use [`bass-m`](https://github.com/elseyf/bass-m), and invoke it with:
```
bass-m \
    ./src/rex-run.gasm \
    -d header_name=rex-run -d header_mapper=0x00 -d header_rom=0x00 -d header_ram=0x00 \
    -o rex-run.gb
```
Fix the resulting rom header with [`gbfix`](https://github.com/elseyf/gbfix) (or any other rom fixing tool)
