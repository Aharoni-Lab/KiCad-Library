# KiCad-Library

KiCad-Library holds the schematics and footprints for all components used in the Aharoni Lab.

## Getting Started

* Clone KiCad-Library to your local computer. We suggest placing it in "documents/KiCad/" where it will be along side your other user created files. You will then need to add the schematic and footprint library paths to KiCad. 
* We suggest configuring a new path as something like "KICAD_AHARONI_LAB" with the path to the location to this repo an then using "KICAD_AHARONI_LAB" for each library path.

### Prerequisites

You will need [KiCad v5.x](http://kicad-pcb.org/) to use these libraries. We also suggest getting the free lite version of [PCB Library Expert](http://www.pcblibraries.com/LibraryExpert/) to generate new footprints to be added to this library.


### Installing
* Clone KiCad-Library to local computer. We suggest placing it in the KiCad documents folder "documents/kicad/".
* To simplify adding each schematic and footprint library to KiCad, we suggest creating a new PATH pointing to the local location of the cloned repo. 
** In Kicad, preferences -> Configure Paths
** "Add"
** Create a name like "KICAD_AHARONI_LAB" along with the path pointing to the root directory of this repo.
* Now you will need to add the name and location of each library to KiCad.
** Click "Symbolic Library Editor"
** Preferences -> Manage Symbol Libraries
** Click "Append Library"
** Add Nickname and Library Path

For example
```
Nickname : .Device
Library Path : ${KICAD_AHARONI_LAB}/Libraries/.Device.lib
```



## Contributing Requirements

* [KiCad library conventions](http://kicad-pcb.org/libraries/klc/) should be followed whenever posisble.
* All footprints should be generated in PCB Library Expert and the footprint file should denote "_M", "_N", "_L" for most, nominal, and least footprint size respectively. Generally we make all footprints that will be assembled with a PnP machine with the least footprint setting to minimize their size.
* Atomic component conventions should be followed whenever you have a specific component and not a generic symbol.
* While KiCad comes with a bunch of part schematics and footprints, all components used in lab should be placed in this KiCad-Library with the correct PCB Library Expert footprint.

## Built With

* [PCB Library Expert](http://www.pcblibraries.com/LibraryExpert/) - All component footprints and 3D step files
* [KiCad](http://kicad-pcb.org/) - PCB EDA


## Authors

* **Daniel Aharoni** - *Initial work* - [DAharoni](https://github.com/DAharoni)

See also the list of [contributors](https://github.com/Aharoni-Lab/KiCad-Library/contributors) who participated in this project.

