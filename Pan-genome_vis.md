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


