# scad-lib

I do a lot of mucking about with Marius Kintel's [OpenSCAD](https://openscad.org), a programmatic 3D modeling tool that's remarkably flexible for highly parameterized geometric shit.

Among other things, it offers support for inclusion of third-party library files, and I rely on a bunch of them for stuff like making screw threads, complex geometry manipulation, and standardized generation of shapes like OpenLock tiles and LEGO bricks. Keeping those libraries up to date and syncing them across my different machines (or setting them up when I build a new machine) is a pain, so I've centralized them all here.

Most libraries have a "core" library file that can be included to access the features. In most cases there's a symlink alias to that file at the root level of this directory, to simplify usage.

Most libraries — because they're available here on GitHub — are included as git submodules. Anything else is checked into the repository itself, license permitting.

## What's here

- [Belfry OpenSCAD Library, V2](https://github.com/revarbat/BOSL2): The granddaddy of geometric manipulation libraries. Its core file is aliased as `bosl.scad`.
- [Boardgame Insert Toolkit](https://github.com/IdoMagal/The-Boardgame-Insert-Toolkit): An all-singing, all-dancing library for building boardgame box inserts with a variety of card and part containers, trays, and so on. Aliazed as `boardgame.scad`
- [PolyGear](https://github.com/dpellegr/PolyGear/): Generates spur and bevel gears as single, self-contained polyhedrons rather than complex boolean objects. Aliased as `polygear.scad`.
- [KeyV2](https://github.com/rsheldiii/KeyV2): Keyboard keycaps and keysets. Aliased as `keys.scad`.
- [LEGO](https://github.com/cfinke/LEGO.scad): Assorted LEGO bricks and plates. Aliased as `lego.scad`.
- [PolyDice](https://github.com/charmaur/PolyDiceGenerator/): Polyhedral dice; most require resin prints to turn out, but larger dice work even with FDM. Aliased as `dice.scad`.
- [DragonLock](https://example.com/): A Jeff Eaton special; generates Dragonlock-compatible bases for tabletop gaming terrain. Aliased as `dragonlock.scad`.
