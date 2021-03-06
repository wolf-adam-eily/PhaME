Installing PhaME
################

PhaME can be installed using conda. If you do not have anaconda or miniconda installed, please do so. Installation of miniconda or anaconda is rather straight forward. After installtion of conda, add channels for bioconda and conda-forge using:
 
 .. code-block:: console
 
    $ conda config --add channels r
    $ conda config --add channels defaults
    $ conda config --add channels conda-forge
    $ conda config --add channels bioconda


Then simply run


.. code-block:: console

    conda install phame

We do recommend creating a separate conda environment for PhaME. You can create a conda environment by:

.. code-block:: console

    $ conda create -n my_env
    $ conda install phame -n my_env



Dependencies
============

Programming/Scripting languages
-------------------------------
* Perl > 5.16

Third party softwares/packages
-------------------------------
* MUMmer version 3.23 - For pairwise alignments of genomes and contigs using NUCmer 
* Bowtie2 version >=2.2.8 - To map reads
* BWA >= 0.7.17 - To map reads
* SAMtools >=1.6 Convert BAM files and other miscs functions.
* FastTree version >=2.1.9 - Construction of phylogenetic tree.
* RAxML version >=8.2.9 - Maximum likelihood construction of phylogenetic tree.
* mafft version >=7.305 - Alignment of protein coding genes for evolutionary analyses.
* pal2nal version >=14 - Converts protein sequence alignment to codon alignments.
* paml version >=4.8 - For evolutionary analyses
* HyPhy version >=2.2 - For evolutionary analyses
* cmake VER >= 3.0.1
* gcc >= 4.9
* bcftools VER >= 1.6 - For calling SNPs.
* bbmap version >= 37.90 -  For picking references using mash

Perl Packages
-------------
* File::Basename = 2.85
* File::Path = 2.09
* Getopt::Long = 2.45
* IO::Handle = 1.28
* Parllel::ForkManager = 1.17
* Statistics::Distributions = 1.02
* Time::BaseName = 2.85
* Time::HiRes = 1.9726
