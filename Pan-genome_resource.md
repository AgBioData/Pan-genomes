# The AgBioData pan-genome resource #

### Brief history ###
In bacteria and viruses, the small genomes and proliferation of complete assemblies lead to the development of a number of construction and analysis methods for looking at the full genetic diversity of an organism, along with visualizations. However, these methods and visualizations don't scale well to the larger and more complex plant and animal genomes. New methods have been developed for the human and human model species pan-genomes, which are helpful for animal pan-genomes, but these methods also don't translate easily to plants as animal genomes lack the genomic and diversity complexities that are found in plant genomes.


### Terminology ###
As the term "pan-genome" means different things to different people, here are definitions used in this resource.

  **annotation**: The outcome of a gene model analysis.
  
  **core gene models**: The set of gene models that appear in all annotations in the pan-genome analysis, with the assumption they are all required. Also called **essential** gene models.
  
  **gene family**: A set of gene models that appear to be the same thing based on sequence similarity and syntenic relationships.
  
  **gene model**: A predicted protein-coding gene.

  **pan-gene**: A collection of gene models from a pan-genome that appear to all be the same thing. It could also include related information such as protein(s), metabolic pathway(s), et cetera.

  **pan-genome**: The sum of all sequence across the genomes/assemblies analyzed, including all variations (SNPs, CNVs, Indels, translocations, inversions).
  
  **pan-genome analysis**: An analysis carried out on a pan-genome.
  
  **rare gene models**: gene models that appear in only one or very few annotations in the pan-genome analysis. Also called **dispensible** gene models.
  
  **variable gene models**: gene models that appear in a subset of annotations in the pan-genome analysis. Also called **accessory** gene models.
  

### What are pan-genomes good for anyway? ###

Interest in pan-genomes has increased rapidly over the past 10 years or so. Considerable progress has been made in the construction and analysis of pan-genomes, though many big problems remain, such as standards and file formats for archiving and sharing the data, useful visualization and browsing software, and, one could argue, a clear understanding of how pan-genomes can be used to further biological knowledge and the improvement of crops and livestock. Sure, pan-genomes are fascinating from a computational perspective, *but what are they good for*?

A good review of how pangenomes have been used in crop improvement
[David Edwards et. al., Pangenomics in crop improvement—from coding structural variations to finding regulatory variants with pangenome graphs. Dec. 2021]
(https://doi.org/10.1002/tpg2.20177)

In short, pan-genomes can help identify differences that make a difference. Studies can be done on multiple scales, ranging from individual genes to local groupings of gene models and rearrangements, to whole pan-genome analyses.

*(Old topic list is below)* \
  **Comparative genomics, evolution, domestication**
  <details>
    <summary>Click for more information</summary>
Analysis of the core, variable, and rare gene models can help reveal information about evolution and domestication.

*[Add: types of analyses, types of datasets, file formats, sample paper, and if available: tutorials]*
  </details>
 
  **Breeding**
  <details>
    <summary>Click for more information</summary>
*[PHG is a good case study for this]*
  </details>
  
  **Gene function**
  <details>
    <summary>Click for more information</summary>
Example showing how this approach can help identify disease resistance genes: \
[Gao, L., Gonda, I., Sun, H. et al. The tomato pan-genome uncovers new genes and a rare allele regulating fruit flavor. Nat Genet 51, 1044–1051 (2019).](https://doi.org/10.1038/s41588-019-0410-2)

*[Add: types of analyses, types of datasets, file formats, and if available: tutorials]*
  </details>
  
  **Assembly and annotation quality control**
  <details>
    <summary>Click for more information</summary>
The construction of core, variable, and rare genes could be used to create a species- or clade-specific sort of BUSCO set for assessing the quality of subsequent genome assemblies and annotations.

*[Add: types of analyses, types of datasets, file formats, sample paper, and if available: tutorials]*
  </details>


<br>
<div style="color:gray">
***Old headings:***

  **Identify core (essential), variable (aka accessory), and rare (aka dispensable) gene models through gene family analyses**
  <details>
    <summary>Click for more information</summary>
The analyses creating gene species- or clad-specific gene families typically look at sequence similarity and synteny. This can be helpful in identifying genes that give a particular plant desireable (or undesireable) traits.

*[Link to paper on definition and construction of these?]* 

Example showing how this approach can help identify disease resistance genes: \
[Gao, L., Gonda, I., Sun, H. et al. The tomato pan-genome uncovers new genes and a rare allele regulating fruit flavor. Nat Genet 51, 1044–1051 (2019).](https://doi.org/10.1038/s41588-019-0410-2)
  </details>
  
  **Comparative genomics, evolution, domestication.**
   <details>
    <summary>Click for more information</summary>
    *[More information goes here.]*
  </details>
 
  **Assessing quality of assemblies and annotations.**
   <details>
    <summary>Click for more information</summary>
    The construction of core, variable, and rare genes could be used to create a species- or clade-specific sort of BUSCO set for assessing the quality of subsequent genome assemblies and annotations.
  </details>
 
  **Genotyping ... to assist breeding?**
   <details>
    <summary>Click for more information</summary>
    *[More information goes here.]*
  </details>
 
  **To both simplify and elaborate information about a species or clade**
   <details>
    <summary>Click for more information</summary>
    *[More information goes here.]*
  </details>
 
  **Practical Haplotype Graphs**
   <details>
    <summary>Click for more information</summary>
    *[More information goes here.]*
  </details>
 
  **Any help with gene function? GWAS? ???**
  <details>
    <summary>Click for more information</summary>
    *[More information goes here.]*
  </details>
</div>


### Analysis software and pipelines ###
Techniques for construction and analysis of pan-genomes is an active field of research. A good review of the state of pan-genome research as of 2020 can be found in [Vernikos GS. A Review of Pangenome Tools and Recent Studies. 2020 May 1. In: Tettelin H, Medini D, editors. The Pangenome: Diversity, Dynamics and Evolution of Genomes. Cham (CH): Springer; 2020. Available from: https://www.ncbi.nlm.nih.gov/books/NBK558826/](http://dx.crossref.org/10.1007/978-3-030-38281-0_4)

[Learn more](Pan-genome_analysis.md)

### Visualizing and browsing pan-genome data ###

Visualization of pan-genome data is a very active field of research, ranging from very complex "hairball" graph displays, to genome-by-genome comparisons on the gene level.

[Learn more](Pan-genome_vis.md)

### For data resources: archiving and presenting pan-genome data ###

Given that construction, analysis, and visualization software is still rapidly evolving, determining how to archive and present the data presents a significant challenge to data resource personnel.

[Learn more](Pan-genome_data.md)
