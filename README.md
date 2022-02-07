![](https://github.com/senselogic/NUBEA/blob/master/LOGO/nubea.png)

# Nubea

E57 point cloud converter.

## Command line

```bash
nubea <options>
```

### Options

```bash
--verbose : show the processing messages
--position-offset <x> <y> <z> : set the loading position offset
--position-scaling <x> <y> <z> : set the loading position scaling
--position-rotation <x> <y> <z> : set the loading position rotation
--position-translation <x> <y> <z> : set the loading position translation
--color-offset <r> <g> <b> <i> : set the loading color offset
--color-scaling <r> <g> <b> <i> : set the loading color scaling
--color-translation <r> <g> <b> <i> : set the loading color translation
--decimation-count <decimation count> : set the loading decimation count
--read-e57-cloud <file path> : read an E57 point cloud
--write-xyz-cloud <file path> <component format> : write an XYZ point cloud
--write-pts-cloud <file path> <component format> : write a PTS point cloud
--write-ptx-cloud <file path> <component format> : write a PTX point cloud
--write-pcf-cloud <file path> <component format> <position bit count> <position precision> : write a PCF point cloud
```

### Point format

```
x : -X
X : +X
y : -Y
Y : +Y
z : -Z
Z : +Z
n : intensity (from -2048 to 2047)
i : intensity (from 0 to 1)
I : intensity (from 0 to 255)
r : red (from 0 to 1)
R : red (from 0 to 255)
g : green (from 0 to 1)
G : green (from 0 to 255)
b : blue (from 0 to 1)
B : blue (from 0 to 255)
```

## Installation

### Linux

*   run `update.sh`
*   run `get.sh`
*   run `make.sh`

### Windows

*   install [Visual C++ 2019 Community](https://docs.microsoft.com/en-us/visualstudio/releases/2019/redistribution#vs2019-download)
*   install [Cmake 3.21](https://github.com/Kitware/CMake/releases/download/v3.21.0-rc3/cmake-3.21.0-rc3-windows-x86_64.msi)
*   run `update.bat`
*   run `XERCES/make.bat`
*   run `make.bat`

## Dependencies

*   [PCF](https://github.com/senselogic/PCF/tree/master/CODE/CPP)
*   [Boost 1.76.0](https://boostorg.jfrog.io/artifactory/main/release/1.76.0/source/boost_1_76_0.7z)
*   [Xerces 3.2.3](https://downloads.apache.org/xerces/c/3/sources/xerces-c-3.2.3.zip)

## Version

0.2

## Author

Eric Pelzer (ecstatic.coder@gmail.com).

## License

This project is licensed under the GNU General Public License version 3.

See the [LICENSE.md](LICENSE.md) file for details.
