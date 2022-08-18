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


