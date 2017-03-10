---
# knit: bookdown::preview_chapter
output: html_document
---



# Overview of experimental methods for generating scRNA-seq data

Development of new methods and protocols for scRNA-seq is currently a very active area. Over the last few years, a large number of different methods have been published. The methods can be categorized in different ways, but the most important is the distinction between full-length and tag-based protocols. The former tries to achieve a uniform read coverage of each transcript. By contrast, tag-based protocols only capture either the 5'- or 3'-end of each mRNA molecule. Another important consideration is the platform where the options are microwell-, microfluidic- and droplet-based.

The choice of quantification method has important implications for what types of analyses the data can be used for. In theory, full-length protocols should provide an even coverage of transcripts, but as we shall see, there are often biases in the coverage. By contrast, tagged protocols will only capture the 5'- or 3'- most end of the RNA molecule. The main advantage of tag-based protocol is that they can be combined with unique molecular identifiers (UMIs) which can help improve the quantification (see chapter X). On the other hand, being restricted to one end of the transcript may reduce the mappability and it also makes it harder to distinguish different isoforms[@Archer2016-zq].

The platform determines how the cells can be selected as well as what kind of additional information besides the sequencing that can be obtained.

For well-based platforms, cells are isolated in each microfluidic well. One advantage of well-based methods can be combined with fluorescent activated cell sorting (FACS), making it possible to select cells based on surface markers. This strategy is thus very useful for situations when one wants to isolate a specific subset of cells for sequencing. Another advantage is that one can take pictures of the cells to


The idea behind droplet based methods is to encapsulate each individual cell inside a nanoliter droplet together with a bead. The bead is loaded with the enzymes required to construct the library. In particular, each bead contains a unique barcode which is attached to all of the reads originating from that cell. Thus, all of the droplets can be pooled, sequenced together and the reads can subsequently be assigned to the cell of origin based on the barcodes. Droplet platforms typically have the highest throughput since the library preparation costs are on the order of .05 USD/cell. Instead, sequencing costs often become the limiting factor and a typical experiment the coverage is low with only a few thousand different transcripts detected[@Ziegenhain2017-cu].