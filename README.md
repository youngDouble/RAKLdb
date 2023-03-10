# Riemerella_anatipestifer_K_locus_Kaptive_db



 This pipline is a Unix-style command-line tool that reports information about capsule polysaccharide synthesis loci and  serovar type for *Riemerella anatipestifer* genome assemblies.

#  Installation

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
git clone https://github.com/katholt/Kaptive

git clone 

```

