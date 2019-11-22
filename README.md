# Some notes on sra-tools usage
It is an outline of sra-tools usage routine. First, the copmpute (instance) is to have enough memory (16G? -- maybe, 8G) ana to have disk space to kepp raw data for at least one experiment. It coukd be 250Gish if we plan to work with fasta.

## Installation
Sra-tools as well the aligner or other tools are very convienient to be installed with conda. First, install conda itself. 
[Miniconda installtion page](https://docs.conda.io/en/latest/miniconda.html "Miniconda installtion page"). Conda suggest to modify the shell prompt after installation. I wuld say no and just add conda/bin (usually, it is ~/mniconda3/bin) to path. Now, install [sra-tools](https://anaconda.org/bioconda/sra-tools "sra-tooks installtion page in conda"), [salmon](https://anaconda.org/bioconda/salmon "salmon installtion page in conda"). etc. You are to do it once for a new user, then sometimes [update conda](https://docs.conda.io/projects/conda/en/latest/commands/update.html) if you like.

## dbGaP accession
Usually, the FastQ file is controlled thing and you are to have access. Technically, it means that you have the keyfile usually, it name is something like prj_NNNNNNN.ngc. NNNNN is a number of dbGaP -- our is 23539. To start working the project, say:

`vdb-config --import prj_23539.ngc`

## FastQ 
Usualle, we do not need all the fatstq files simultaneously
