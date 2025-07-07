# Squirrel genomics
Code repository for the squirrel genomics project

## 1. Open screen session

Open a screen session to run the pipeline in the background. The session has the same name as the directory for the sake of simplicity.

```sh
screen -S 2025_squirrel_genomics
```

## 2. Prepare directory with pipeline

Clone the AlberdiLab genotyping pipeline repository to the server.

```sh
git clone https://github.com/alberdilab/genotyping
mv genotyping 2025_squirrel_genomics
cd 2025_squirrel_genomics
```

Download Snakemake wrappers to avoid connection issues.

```sh
git clone --depth 1 --branch v7.2.0 https://github.com/snakemake/snakemake-wrappers.git  workflow/wrappers/v7.2.0
```

## 3. Fetch sequencing data

Download raw sequencing data from the EHI repository. This takes a while.

```sh
cd resources/reads
wget -i reads.csv
```

## 4. Download reference genome

Download the red squirrel reference genome from the NCBI.

```sh
Add code
```

## 5. Launch pipeline

Launch Snakemake pipeline and wait until the final variant calling file is generated.

```sh
Add code
```
