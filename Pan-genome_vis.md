# Visualizing Pan-Genomes
[Return to top page](Pan-genome_resource.md)

Visualization of pan-genome data is a very active field of research. Visualization approaches range from very complex "hairball" graph displays, to comparisons on the gene level across multiple genomes, and from all-by-all views to pair-wise comparisons.

A good example of a pan-genome browser comes from the Mouse Genomics Informatics resource, the mouse 
[Multi-Genome Viewer](http://www.informatics.jax.org/mgv).

Visualization and browsing of the rice pan-genome is implemented in [JBrowse](http://www.ricesuperpir.com/web/riceHubAssembly).

A slide deck from 2022 summarizing pan-genome analysis and visualization software can be seen [here](https://drive.google.com/file/d/1rU0tzl2uIhP9xk8egJX4IzTPQC3QJNn8/view?usp=sharing). The tools from these slides an others are summarized below.

## Bandage Fork
[Bandage](https://rrwick.github.io/Bandage/)[1] is a tool originally designed for the visualization of de novo assembley graphs. With the advent of the pangenome and [Bandage no longer in active development](https://github.com/rrwick/Bandage#2022-update), a fork of Bandage has been created that supports pangenome graph visualization: [https://github.com/asl/BandageNG](https://github.com/asl/BandageNG). The key feature of this fork is that it supports GFA files with embedded paths. This allows users to visualization the paths that particular chromosomes/assemblies take through a pangenomic graph, allowing them to visually identify the preservation and variation of sequences within chromosomes/assemblies of interest.

Pros:
* Visualizes pangenome graphs
* Visualizes paths embedded in a pangenome graph
* Can BLAST search node sequences against a BLAST database
* Can build a BLAST database for the graph and search its sequences 

Cons:
* Not very scalable
    * Often requires visualizing one chromosome or slices of a chromosome individually
    * Or requires the smoothing of the graph to reduce complexity
* The drawing algorithm never draws a graph the same way twice

[1] Ryan R. Wick, Mark B. Schultz, Justin Zobel, Kathryn E. Holt,  Bandage: interactive visualization of de novo genome assemblies, Bioinformatics, Volume 31, Issue 20, 15 October 2015, Pages 3350–3352, [https://doi.org/10.1093/bioinformatics/btv383](https://doi.org/10.1093/bioinformatics/btv383)


## GfaViz

[GfaViz](https://github.com/ggonnella/gfaviz)[2] is a GFA viewer that explicitly supports variation graphs, i.e. pangenomic graphs. It has a variety of coloring and layout options. Paths embedded in graphs (such as pangenomes) are distinguished using different graph edge and node outline colors. Conventiently, GfaViz supports exporting pictures of graphs as SVG files.

Pros:
* Visualizes pangenome graphs
* Visualizes paths embedded in a pangenome graph
* Visualization is customizable via user interaction

Cons:
* Not under active development
* No built-in sequence search
* Limited documentation

[2] Giorgio Gonnella, Niklas Niehus, Stefan Kurtz,  GfaViz: flexible and interactive visualization of GFA sequence graphs, Bioinformatics, Volume 35, Issue 16, 15 August 2019, Pages 2853–2855, [https://doi.org/10.1093/bioinformatics/bty1046](https://doi.org/10.1093/bioinformatics/bty1046)


## Panache
[Panache](https://github.com/SouthGreenPlatform/panache)[3] is a web-based interface designed for the visualization of linearized pangenomes. It can be used to show presence/absence information of pangenomic blocks of sequence or genes in a genome browser-like display. It does not provide a method for linearizing the genomes and the data formats it consumes are non-standard.

Pros:
* Linearized viewer is intuitive to usres familiar with genome browsers
* Interactive features allow for easy exploration of linearized pangenome

Cons:
* No method for generating input files provided
* Doesn't scale well, especially for complex genomes
* Linearized representation isn't great for representing genomes with complex structures and rearrangements

[3] Éloi Durant, François Sabot, Matthieu Conte, Mathieu Rouard,  Panache: a web browser-based viewer for linearized pangenomes, Bioinformatics, Volume 37, Issue 23, 1 December 2021, Pages 4556–4558, [https://doi.org/10.1093/bioinformatics/btab688](https://doi.org/10.1093/bioinformatics/btab688)


## Anvi'o
[Anvi'o](https://anvio.org/)[4] is an analysis and visualization platform for 'omics data, including pipelines for microbial pangenomic data. These pipelines can generate informative visualizations, such as Circos diagrams of mean coverage and UpSet plots of gene content.

Pros:
* Pipelines are well tested and work on common file types
* Visualizations are useful

Cons:
* Only scales to microbial genomes
* Anvi'o is a large suit of tools with a steep learning curve

[4] Eren AM, Esen ÖC, Quince C, Vineis JH, Morrison HG, Sogin ML, Delmont TO. 2015. Anvi’o: an advanced analysis and visualization platform for ‘omics data. PeerJ 3:e1319 [https://doi.org/10.7717/peerj.1319](https://doi.org/10.7717/peerj.1319)


## PanX
[PanX](https://github.com/neherlab/pan-genome-analysis)[5] is a software package for microbial pangenome analysis, visualization, and exploration. It includes pipelines for aligning and clustering protein sequences, building phylogenies, building SNP trees, identifying gene presence/absence, and clustering genes into the core and pan. PanX also includes a variety of visualizations of these analyses.

Pros:
* Performs a variety of useful analyses and visualizes their results
* All visualizations are given in a single view that makes cross comparison easy

Cons:
* Only scales to microbial genomes
* Not under active development

[5] Wei Ding, Franz Baumdicker, Richard A Neher,  panX: pan-genome analysis and exploration, Nucleic Acids Research, Volume 46, Issue 1, 9 January 2018, Page e5, [https://doi.org/10.1093/nar/gkx977](https://doi.org/10.1093/nar/gkx977)


## GCV (Genome Context Viewer)
[GCV](https://github.com/legumeinfo/gcv)[6] is a visual data-mining tool that allows users to search across multiple providers of genome data for regions with similarly annotated content that may be aligned and visualized at the level of their shared functional elements. Visualizations include micro-synteny tracks, macro-synteny (chromosome) blocks, pairwise dots plots, and Circos diagrams.

Pros:
* Only requires annotated genomes
* All analyses are performed on-the-fly with tuneable algorithms
* Actively developed

Cons:
* Only operates at the genic level
* Microservices architecture is complex

[6] Alan Cleary, Andrew Farmer,  Genome Context Viewer: visual exploration of multiple annotated genomes using microsynteny, Bioinformatics, Volume 34, Issue 9, 01 May 2018, Pages 1562–1564, [https://doi.org/10.1093/bioinformatics/btx757](https://doi.org/10.1093/bioinformatics/btx757)


## Sequence Tube Maps
[Sequence Tube Maps](https://github.com/vgteam/sequenceTubeMap)[7] is a tool for visualizing genomic sequence graphs built using vg, i.e. acyclic graphs. The visualization is akin to multiple sequence alignments but better handles structures like indels.

Pros:
* Easy to interpret if already familiar with multiple alignment visualizations
* Supports vg file types
* Interactive
* Actively developed

Cons:
* Doesn't scale to large genomes
* Linear requirement limits what genomes can be visualized

[7] Wolfgang Beyer, Adam M Novak, Glenn Hickey, Jeffrey Chan, Vanessa Tan, 
Benedict Paten, Daniel R Zerbino,  Sequence tube maps: making graph 
genomes intuitive to commuters, Bioinformatics, Volume 35, Issue 24, 15 December 2019, Pages 5318–5320, [https://doi.org/10.1093/bioinformatics/btz597](https://doi.org/10.1093/bioinformatics/btz597)


## MoMI-G
[MoMI-G](https://github.com/MoMI-G/MoMI-G)[8] is a Modular Multi-scale Integrated Genome Graph Browser, hence the name. It integrates Circos, Sequence Tube Map, and data tables into a single view for simultaneous, multi-scale analysis of you graphical pangenomic data.

Pros:
* Consumes standard file types
* Provides multiple, complementary visualizations
* Actively developed

Cons:
* Although it scales to large genomes, it does so by only viewing specific slices of the genomes

[8] Yokoyama, T.T., Sakamoto, Y., Seki, M. et al. MoMI-G: modular multi-scale integrated genome graph browser.
BMC Bioinformatics 20, 548 (2019). [https://doi.org/10.1186/s12859-019-3145-2](https://doi.org/10.1186/s12859-019-3145-2)


## PGV (Pangenome Graph Viewer)
[PGV](https://github.com/ucrbioinfo/PGV)[9] is a pipeline for the reference-agnostic representation and visualization of pangenomes. The pipeline is based on progressiveMauve and the visualizations are based the concensus ordering of the computed blocks.

Pros:
* Reference-agnostic
* Can handle large genomes

Cons:
* Not under active development
* Use of progressiveMauve limits scalability
* Species with complex structures could be hard to interpret in context of concensus ordering

[9] Liang, Q., Lonardi, S. Reference-agnostic representation and visualization of pan-genomes.
BMC Bioinformatics 22, 502 (2021). [https://doi.org/10.1186/s12859-021-04424-w](https://doi.org/10.1186/s12859-021-04424-w)
