
## Patterns and features on genomes in R: Biostrings, BSgenome and GenomicRanges.
### 'FLS' R group - October 2015
### Dave Gerrard

Biostrings, BSgenomes and GenomicRanges.

### PRE-REQUISITES --------------------------------
Multiple bioconductor packages but should get them all by doing this. 


```{r, eval=FALSE}
source("https://bioconductor.org/biocLite.R")
# Try http if https is not available
biocLite("BSgenome.Scerevisiae.UCSC.sacCer3")    
# 'should' also install Biostrings, BSgenomes and GenomicRanges if not already installed.
```
### The Plan. --------------------------------------
Find instances of a DNA-sequence motif in a genome that also have evidence of binding from a ChIP-seq experiment.

1. Biostrings
2. BSgenome
3. GenomicRanges

The tutorial is in the script [BSgenome.BioStrings.bioC.R](BSgenome.BioStrings.bioC.R). You will need to download some data before you start (see below).


### Data ---------------------------
Tutorial uses a table of genomic ChIP-seq peaks from [Zheng et al., 2010, Nature](http://www.nature.com/nature/journal/v464/n7292/full/nature08934.html)

The data table [GSE19635_s96a_peaks.txt](GSE19635_s96a_peaks.txt) was downloaded from [GEO](http://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE19635) and uncompressed. 


