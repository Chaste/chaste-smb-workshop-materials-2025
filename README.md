# Chaste Tutorial at 2025 SMB Meeting 

A directory of materials for the July 2025 Chaste Tutorial at the OPEN VT workshop in Edmundton, Canada.

The main Chaste repository can be found [here](https://github.com/Chaste/Chaste).

## Prerequesites ##

Before the workshop you will need to download and install Docker (and other useful tools), and download the chaste docker container (this contains the source code you will need).

* Install [Docker](https://www.docker.com/) and allocate it at least 4GB RAM
* On the command line run the following: ``` docker run -it --init --rm -v chaste_data:/home/chaste chaste/release ``` (or one of the commands below to view output)
 * This is your terminal on Chaste we will work in here in the workshop.
* To make things easier you should also Install
 * [VSCode](https://code.visualstudio.com/) for editing code and
 * [Paraview](https://www.paraview.org/) for visualisation.


## Mounting output in Windows

```
docker run -it --init --rm -v chaste_data:/home/chaste -v C:\Projects\output:/home/chaste/output chaste/release
```

## Mountung output in macOS

```
docker run -it --init --rm -v chaste_data:/home/chaste -v "${PWD}"/output:/home/chaste/output chaste/release
```

## Visualising with Paraview
UserTutorials/VisualizingWithParaview

## Tasks 
* https://chaste.github.io/docs/user-tutorials/
  * Where to start with cell-based simulations:
    * UserTutorials/CellBasedDemo - a quick introduction to the basics of cell-based simulations in Chaste.
    * UserTutorials/VisualizingWithParaview
  * Running basic simulation types:
    * UserTutorials/RunningMeshBasedSimulations - the first type of cell-based simulation included in Chaste, start here!
    * UserTutorials/RunningNodeBasedSimulations - includes details of how to simplify cell-based tests
    * UserTutorials/RunningVertexBasedSimulations - includes adding boundary conditions and removing cells from simulations
    * UserTutorials/RunningPottsBasedSimulations - lattice-based simulations
    * UserTutorials/RunningImmersedBoundarySimulations - immersed boundary simulations


