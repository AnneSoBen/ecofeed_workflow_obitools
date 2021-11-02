# workflow_obitools

## About

This is a snakemake workflow based on the obitools suite of programs analyzes DNA metabarcoding data.

Sequence analysis is performed with cutadapt (Martin, 2011), sumaclust (Mercier et al. 2013) and obitools softwares (Boyer et al. 2016), through a Snakemake pipeline (Molder et al. 2021).

## Usage

The pipeline is meant to be executed on a computing cluster running with SLURM for now.

To run the workflow in a single command on the cluster:

```
sbatch sub_smk.sh
```

Two configuration files can be modified: `workflow/cluster.yaml` that sets up the ressources avaiable for each rule, and `config/config.yaml` where you can edit the values of the parameters used by the rules.
