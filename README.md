# SRA Explorer Tutorial
Welcome! This repo serves as a tutorial for using the web tool SRA Explorer written by Phil Ewels. 

## Description
SRA Explorer is a GUI tool that streamlines the process of downloading data from the SRA website in the form of .sra or .fastq files. 

## Tutorial

### Link to Tool

* SRA explorer can be found at this address: [SRA Explorer](https://sra-explorer.info/)

### Running the Program

* SRA Explorer allows you to search for keywords/parameters or accession numbers.
* You can search for some of the accession numbers listed below.
<img width="1044" alt="image" src="https://github.com/nshanbhag123/sra_explorer_tutorial/assets/70123134/f491387a-89b7-4d07-b205-322eccdc52a5">

* You can also simply enter the type of data you are looking for. 
<img width="1038" alt="image" src="https://github.com/nshanbhag123/sra_explorer_tutorial/assets/70123134/42de334b-ad93-41ef-93e3-21d6656e39b9">

### Results
* SRA explorer will return your search with the best hits. You can further filter out the results by checking the entries you want to download.
* Once you have finished selecting, click add to collection in the top right corner.
* If you are done, you can click the shopping cart in the top right corner to check out. If not, you can continue adding datasets to your cart.
<img width="1096" alt="image" src="https://github.com/nshanbhag123/sra_explorer_tutorial/assets/70123134/499a2dd2-dd04-453b-8f93-c9343fc339af">


### Downloading the data
* SRA explorer provides many options to download .fastq or .sra files.
  <img width="1087" alt="image" src="https://github.com/nshanbhag123/sra_explorer_tutorial/assets/70123134/2dd3e2ad-5e7d-4158-bef0-813693b9e17f">
* For a few fastq files, I would recommend using the raw fastq download URL files. You can use wget in your terminal to retrieve the fastq file associated with each run. 
 ```
wget ftp://ftp.sra.ebi.ac.uk/vol1/fastq/SRR141/057/SRR14122857/SRR14122857_1.fastq.gz -P /path/to/your/output/directory
```
* For copius amounts of fastq files, I would recommend using the bash script to download fastq files
  <img width="1077" alt="image" src="https://github.com/nshanbhag123/sra_explorer_tutorial/assets/70123134/84fb45c9-3ddc-4e03-a293-1cf9dae8f48e">
* First, download the bash script. Then, add executable permissions to the script and run.
```
chmod +x /path/to/bash/download/script
```
* To run the script
```
./path/to/bash/download/script
```
* If you are using Apsera, Cluster Flow, or bcbio for downstream applications, you can use wget to apply the same steps.
* If you want the .sra file, you can also either use wget or the bash script to download your files. 
  <img width="1070" alt="image" src="https://github.com/nshanbhag123/sra_explorer_tutorial/assets/70123134/b8f8ae90-2acd-4489-a58b-7b134e0afd73">


## Authors

Contributors names and contact info

* Phil Ewels [@tallphil](https://twitter.com/tallphil)

## Version History

* 1.0


## Acknowledgments

Credits to Phil Ewels
* [SRA Explorer](https://sra-explorer.info/)
