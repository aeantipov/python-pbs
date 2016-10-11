#### python-pbs
A python module that helps with submitting jobs to different supercomputers. The detailed wrapper is cluster-dependent, so different modules for different clusters are collected here along with generic prototypes for OpenPBS and Torque job management systems. The main two commands are `submit_serial(command, job name, account to use, ...) ` and `submit_mpi(command, nprocs, job name, ...)`.

See `clusters` for some known cluster implementations and `examples` for usage examples.

- `pbs_openpbs.py` - OpenPBS wrapper.
- `pbs_torque.py` - TORQUE PBS wrapper.

##### Usage 
The best way to use it is to create a directory somewhere in home location, say `${HOME}/pythonmodules` and add the line 
`export PYTHONPATH=${HOME}/pythonmodules:$PYTHONPATH` to `.bash_profile`. Afterwards any python script will find this module automatically.
