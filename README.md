# Riemerella anatipestifer K locus Database

This repository is a database of capsule polysaccharide synthesis loci (K-loci) for *Riemerella anatipestifer*, which is compatible with Kaptive and can be used for serovar (K-loci) prediction of *Riemerella anatipestifer* genome assemblies.

##  Installation

To ensure stable operation of the workflow, we recommend installing the following dependencies using [`conda`](https://conda.io/projects/conda/en/latest/user-guide/install/index.html):

- [Kaptive](https://github.com/katholt/Kaptive)
- [Python 3](https://www.python.org/downloads/) 

```bash
# activate base environment
source ~/anaconda3/bin/activate
# Create a conda environment named Kaptive_ra and install biopython, blast (for Kaptive), and fastani
conda create -n Kaptive_ra -c bioconda -c conda-forge biopython=1.70=np112py36_1 
blast=2.2.31=pl526he19e7b1_5 fastani=1.33=h0fdf51a_1
# or create conda environment from the *.yaml file
#conda env create  -n Kaptive_ra  -f  Riemerella_anatipestifer_K_locus_Kaptive_db_conda_install.yml

# activate Kaptive_ra 
conda activate Kaptive_ra
# clone Kaptive v2.0.6 
#git clone https://github.com/katholt/Kaptive
cd Kaptive
git clone https://github.com/youngDouble/RAKLdb
```

## How to run

The **Riemerella anatipestifer K locus database** is compatible with `Kaptive` and can be used as described on the [Kaptive homepage](https://github.com/katholt/Kaptive/wiki/How-to-run).

```bash
# activate Kaptive_ra environment
source ~/anaconda3/bin/activate Kaptive_ra
./Kaptive/kaptive.py -a test_ra_assemble.fna -t 30 -k ./Kaptive/Riemerella_anatipestifer_K_locus_Kaptive_db/Riemerella_anatipestifer_K_locus_primary_reference.gbk -g ./Kaptive/Riemerella_anatipestifer_K_locus_Kaptive_db/Riemerella_anatipestifer_wzx_wzy.fasta -o test 

```



## Citation

If you use the *Riemerella anatipestifer* K locus databases in your research, please cite these papers:

- [Genome-wide association study reveals serovar-associated genetic loci in *Riemerella anatipestifer*. BMC Genomics, 2024](https://doi.org/10.1186/s12864-024-09988-4)
- [Identification of *Klebsiella* capsule synthesis loci from whole genome data. *Microbial Genomics* (2016).](http://mgen.microbiologyresearch.org/content/journal/mgen/10.1099/mgen.0.000102)
- [Kaptive 2.0: updated capsule and LPS locus typing for the *Klebsiella pneumoniae* species complex. *Microbial Genomics* (2022).](https://doi.org/10.1099/mgen.0.000800)

