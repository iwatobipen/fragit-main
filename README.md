# FragIt

FragIt is a python based tool that allows you to quickly fragment ["any"](http://openbabel.org/docs/2.3.0/FileFormats/Overview.html) molecule and use the produced output file as an input file in quantum chemistry programs that supports such fragment based methods.

FragIt was made out of the need to quickly benchmark many different molecules while developing a new fragment based method and is now being released in the hope that it is useful for others.

Currently, the only supported method is the [fragment molecular orbital](http://en.wikipedia.org/wiki/Fragment_Molecular_Orbital) method in [GAMESS](http://www.msg.ameslab.gov/gamess/index.html), but new output writers can be added easily to support other methods and programs.

There is also an [online-version available](http://www.fragit.org/) which requires only a browser and Java.

## Obtaining FragIt

Since you found this file, it is obvious that you also found the source code. You can obtain the latest version from [github](https://www.github.com/FragIt/fragit-main) where [tagged releases](https://github.com/FragIt/fragit-main/releases) are also available.

## Installing FragIt

FragIt is a python library and installation is quite straight forward

    python setup.py build
    python setup.py install

to install it in the default locations. To install it in a custom location, you can run the following

    python setup.py build
    python setup.py install --prefix=/path/to/custom/installation

## Running FragIt

in a terminal, you can type

    fragit

to see its help message.

See the [wiki](https://www.github.com/FragIt/fragit-main/wiki) for more examples of how to use FragIt.

## Requirements

In order to run FragIt, you *need* the following installed on your system:

* The FragIt source code, look above for information on how to obtain it
* [Open Babel](http://www.openbabel.org) 2.3 or newer with [python language bindings](http://openbabel.org/docs/dev/Installation/install.html#compile-language-bindings) enabled.
* [Numpy](http://numpy.scipy.org) 1.5 or newer.
* [Python](http://www.python.org) version 2.4 or later (not 3.X)
