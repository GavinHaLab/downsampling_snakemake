# downsampling_bam_paired_snakemake

A snakemake to downsample reads from a bam file, following GATK best practices. 

This repository contains all the folders needed to run the snakemake. logs/cluster/ currently contains a placeholder file because GitHub does not allow empty folders, but after copying this repository structure to the server, this placeholder file can be removed from the server.

To run:

1) update config/samples.yaml and config/config.yaml as per the directions in those files

2) load all modules listed in downsampling_bam_paired.snakefile

3) verify all paths are correct for your application

4) launch snakemake from directory containing the snakemake file with command referenced downsampling_bam_paired.snakefile (with -np) for a dry run which will look for errors and list out all necessary jobs. If no errors and jobs look correct

5) relaunch snakemake with command referenced in downsampling_bam_paired.snakefile without -np

6) snakemake steps will be launched as jobs to the cluster at the Fred Hutchinson Cancer Research Center.
