The mba package can be used to analyze HDF5 container format basecalled files. It is specifically tailored for Oxford Nanopore Reads.

###Requirements
    git
    python 2.7
    pip/virtualenv (see below)

###Installation

To install the code run:

    git clone git://github.com/mitenjain/mba.git
    cd mba
    git pull
    git submodule update --init
    make
This will build the code. 

###Creating a virtual environment to handle python dependencies

mba uses PyPore and yahmm packages, that individualy require a number of python packages. The system python could be used if these dependencies are present. Otherwise, a virtual environment can be created by running the following command in the mba base directory:

    virtualenv --no-site-packages --distribute env && source env/bin/activate && pip install -r requirements.txt

Creation of a virtual environment requires that machine has an existing installation of pip and virtualenv.
