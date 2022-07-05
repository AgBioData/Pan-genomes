# The AgBioData pan-genome resource #

<table style="border:none">
  <tr>
    <td valign="top">
      <h3>Brief history</h3>
      In bacteria and viruses, the small genomes and proliferation of complete assemblies lead to the development of a number of construction and analysis methods for looking at the full genetic diversity of an organism, along with visualizations. However, these methods and visualizations don't scale well to the larger and more complex plant and animal genomes. New methods have been developed for the human and human model species pan-genomes, which are helpful for animal pan-genomes, but these methods also don't translate easily to plants as animal genomes lack the genomic and diversity complexities that are found in plant genomes.
    </td>
    <td valign="top" style="white-space:nowrap">
      <h4>Table of contents</h4>
      <a href="#terminology">Terminology</a><br>
      <a href="#uses">What are pan-genomes good for</a><br>
      <a href="#analysis">Analysis software and pipelines</a><br>
      <a href="#viz">Visualizing and browsing pan-genomes</a><br>
      <a href="#archive">Archiving and presenting pan-genome data</a>
    </td>
  </tr>
</table>


<a name="terminology"></a>
### Terminology ###
As the term "pan-genome" means different things to different people, here are definitions used in this resource.

  **annotation**: The outcome of a gene model analysis.
  
  **core gene models**: The set of gene models that appear in all annotations in the pan-genome analysis, with the assumption they are all required. Also called **essential** gene models.
  
  **gene family**: A set of gene models that appear to be the same thing based on sequence similarity and syntenic relationships.
  
  **gene model**: A predicted protein-coding gene.

  **pan-gene**: A collection of gene models from a pan-genome that appear to all be the same thing. It could also include related information such as protein(s), metabolic pathway(s), et cetera.

  **pan-genome**: The sum of all sequence across the genomes/assemblies analyzed, including all variations (SNPs, CNVs, Indels, translocations, inversions).
  
  **pan-genome analysis**: An analysis carried out on a pan-genome.
  
  **rare gene models**: gene models that appear in only one or very few annotations in the pan-genome analysis. Also called **dispensible** or **orphan** gene models.
  
  **variable gene models**: gene models that appear in a subset of annotations in the pan-genome analysis. Also called **accessory** gene models.
  

<a name="uses"></a>
### What are pan-genomes good for anyway? ###

Interest in pan-genomes has increased rapidly over the past 10 years or so. Considerable progress has been made in the construction and analysis of pan-genomes, though many big problems remain, such as standards and file formats for archiving and sharing the data, useful visualization and browsing software, and, one could argue, a clear understanding of how pan-genomes can be used to further biological knowledge and the improvement of crops and livestock. Sure, pan-genomes are fascinating from a computational perspective, *but what are they good for*?

In short, pan-genomes can help identify differences that make a difference. Studies can be done on multiple scales, ranging from individual genes to local groupings of gene models and rearrangements, to whole pan-genome analyses.

  **Comparative genomics, evolution, domestication**
  <details>
    <summary>Click for more information</summary>
Analysis of the core, variable, and rare gene models can help reveal information about evolution and domestication.

*[Add: types of analyses, types of datasets, file formats, sample paper, and if available: tutorials]*
  </details>
 
  **Breeding**
  <details>
    <summary>Click for more information</summary>
    
Pan-genomes have been used successfully in breeding programs. This paper describes how pan-genomes have revealed extensive genome content variation among individuals within a species: [Rafael Della Coletta et. al., How the pan-genome is changing crop genomics and improvement. January 2021](https://doi.org/10.1186/s13059-020-02224-8)

One common approach makes use of the Practical Haplotype Graph ([ES Buckler et. al., The Practical Haplotype Graph, a platform for storing and using pangenomes for imputation. 2021](https://doi.org/10.1101/2021.08.27.457652))

Some examples:

Improved heritablility in tomato from 0.33 to 0.41 through analyses of 838 genomes ([Yao Zhou et. al., Graph pangenome captures missing heritability and empowers tomato breeding. June 2022](https://doi.org/10.1038/s41586-022-04808-9))

The barley pan-genome makes previously hidden genetic variation accessible to genetic studies and breeding ([Nils Stein et. al., The barley pan-genome reveals the hidden legacy of mutation breeding. November 2020](https://doi.org/10.1038/s41586-020-2947-8))

Crop wild relatives possess unearthed genetic diversity that has been lost during domestication and breeding ([David Edwards et. al. Super-Pangenome by Integrating the Wild Side of a Species for Accelerated Crop Improvement. Febuary 2020](https://doi.org/10.1016/j.tplants.2019.10.012))

   </details>
  
  **Gene function**
  <details>
    <summary>Click for more information</summary>
One approach to determining gene function is to construct pan-genes that include assemblies and annotations that contain characterized genes with the hope that all members of a pan-gene are likely to be serving the same function.

Example showing how pan-genome analyis helped identify disease resistance genes: \
[Gao, L., Gonda, I., Sun, H. et al. The tomato pan-genome uncovers new genes and a rare allele regulating fruit flavor. Nat Genet 51, 1044–1051 (2019).](https://doi.org/10.1038/s41588-019-0410-2)
  
As a pangenome captures all gene variants found in the sequenced individuals, it is possible to identify a subset of individuals representing gene absence as well as each diverse haplotype. This subset of individuals can then be assessed to determine the impact of this diversity on crop traits. Pangenomes can also identify genes that lack significant haplotype diversity. In these cases, teh introduction of diversity through mutagenesis or genome editing may be required to assess gene function.

*[Add: types of analyses, types of datasets, file formats, and if available: tutorials]*
  </details>
  
  **Assembly and annotation quality control**
  <details>
    <summary>Click for more information</summary>
The construction of core, variable, and rare genes could be used to create a species- or clade-specific sort of BUSCO set for assessing the quality of subsequent genome assemblies and annotations. Knowledge of the gene content of a species can support the annotation of related species given  that the majority of gene models are likely to be conserved between closely related species.

*[Add: types of analyses, types of datasets, file formats, sample paper, and if available: tutorials]*
  </details>


<a name="analysis"></a>
### Analysis software and pipelines ###
The construction and analysis of pan-genomes remains a young and rapidly changing field. Nonetheless, well-documented and reproducible pipelines are needed, but rarely found. Pipelines that are developed quickly become outdated with new developments in genome assembly and sequencing technology.

[Learn more](Pan-genome_analysis.md)

<a name="viz"></a>
### Visualizing and browsing pan-genome data ###
Visualization of pan-genome data is a very active field of research. Visualization approaches range from very complex "hairball" graph displays, to comparisons on the gene level across multiple genomes, and from all-by-all views to pair-wise comparisons.

[Learn more](Pan-genome_vis.md)

<a name="archive"></a>
### For data resources: archiving and presenting pan-genome data ###

Given that construction, analysis, and visualization software is still rapidly evolving, determining how to archive and present the data presents a significant challenge to data resource personnel.

[Learn more](Pan-genome_data.md)


