This is an [Apptainer](https://apptainer.org/) definition file intended to create an Ubuntu 22.04 system with NVIDIA Cuda 12.1 support. It's intended to be used on the [Digital Research Alliance of Canada](https://alliancecan.ca/en)'s compute stack (I test on Cedar, but it should probably work on any of DR's machines).

To build:

[Install](https://apptainer.org/docs/admin/main/installation.html) Apptainer into your OS.

Build with `apptainer build ubuntu-nvidia-12.1.sif ubuntu-nvidia-12.1.def` 

Note that Digital Research's CUDA level may change, in which case I'll have to rebuild this with the appropriate CUDA. To check the CUDA level on any machine that has CUDA support, run the command `nvidia-smi -q`. 
