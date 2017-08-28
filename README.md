# LVPP sigma-profile database

This is the LVPP sigma-profile database for COSMO-based models. It currently contains information for more than **1700 molecules**.

Currently, in this repository we only provide the COSMO apparent surface charges computed either with
[GAMESS](http://www.msg.ameslab.gov/gamess/) or [MOPAC](http://openmopac.net/).

You will still need other code to actually compute activity coefficients or other properties with models like COSMO-RS or COSMO-SAC.

## Citing
We kindly ask you to cite this work as "An open and extensible sigma-profile database for COSMO-based models",
F. Ferrarini, G. B. Flores, A. R. Muniz, and R. de P. Soares (2017), *still under review*.

## Using
The *processed* database is made available in ZIP files, check the [releases](http://github.com/lvpp/sigma/releases).
Just download one of the release files, uncompress and look for the molecule you need.

Currently we have the following releases:
* HF+TZVP using GAMESS
* POA1 using MOPAC

## Extending the database

There are different methods to extend the database.

### Ask LVPP to add new molecules

Just create and [new issue](https://github.com/lvpp/sigma/issues)
and describe the molecules you need that are missing.
If possible also attach a **3D mol** file for each molecule you want added.
It can take a while until we process your request.

### Process your own molecules

If you can't wait for us to process your molecules (or if you don't want to)
you can can **process** your own molecules.

Just **clone** or download this repository and then
please check either the [GAMESS](https://github.com/lvpp/sigma/tree/master/GAMESS)
or the [MOPAC](https://github.com/lvpp/sigma/tree/master/MOPAC) folders for instructions
on how to process your own molecules.

Our instructions are for Ubuntu Linux 16.04 or superior. They probably should also
work on other similar systems.

Regardless if you will use GAMESS or MOPAC,
our provided instructions depend on the following packages:
```
$ sudo apt-get install scons openbabel libiomp5
```

## License

The LVPP sigma-profile database and all the documents distributed in this repository are distributed under the terms
of the [MIT License](https://github.com/lvpp/sigma/blob/master/LICENSE).