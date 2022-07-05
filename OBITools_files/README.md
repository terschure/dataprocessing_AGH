# OBITools demultiplexing
The raw data for this project is the result of one sequencing pool, containing plant amplicons of all of the samples.
The first steps in the dataprocessing require a sample description file for the demultiplexing using OBITools *ngsfilter*:

 - ngsfilter_description_agh.txt

The sample names used in these sample descriptions contain the following information:
[sample_number]\_[sample_type]\_[replicate]

- [sample_type] can be 's' for sample, 'pnc' for PRC negative control or 'enc' for extraction negative control
- [replicate] can be '1' to '6' and represent the different PCR replicates used for amplification
