# sedaDNA dataprocessing Aghitu-3 cave
The files and scripts used for processing the DNA metabarcoding data from the cave sediment samples collected at Aghitu-3

## OBITools ngsfilter
The raw data for this project is the result of one sequencing pool, containing plant amplicons of all of the samples.
The first steps in the dataprocessing require a sample description file for the demultiplexing using OBITools *ngsfilter*:

 - ngsfilter_description_agh.txt

The sample names used in these sample descriptions contain the following information:
[sample_number]\_[sample_type]\_[replicate]

- [sample_type] can be 's' for sample, 'pnc' for PRC negative control or 'enc' for extraction negative control
- [replicate] can be '1' to '6' and represent the different PCR replicates used for amplification

## R filtering stages 1 and 2
After the first processing steps using OBITools, the data was filtered in R version 4.1.0.
This was done in two distinct stages, the first stage includes standard initial filtering steps. The resulting data were then checked by a taxonomic expert. Several taxonomic assignments were manually adjusted and sequences identified that were unlikely for the region at the time. Additional filtering steps were performed in stage two.

 - Rfiltering_1.Rmd
 - Rfiltering_2.Rmd
