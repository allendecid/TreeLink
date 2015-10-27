# TreeLink
Data Integration, Clustering and Visualization of Phylogenetic Trees.

Treelink is a platform-independent software for linking datasets to trees, taxon clustering and phylogenetic analysis based on topology.

The application allows an automated integration of datasets to trees resulting in annotated visualizations displaying the distribution of selected data attributes in branches and nodes. Genomic and proteonomic sequences can also be linked to the tree and extracted from internal nodes and leafs.

A novel clustering algorithm to simplify trees and display the most divergent clades was also developed. Phylogeographic inference and plotting based on maximum parsimony and maximum likelihood for ancestral reconstruction is also comprehended. File support includes the most popular formats like newick and csv. Exporting visualizations as images, cluster outputs and genomic sequences is supported.

To use on a desktop, download the files and Node WebKit. Add the files to the Node WebKit project folder and run the executable.

To use on a website, download the html files ending with *web.html, the js and css folder and upload them to a server. 

To visualize the tree, it is necesarry to add the tag `<div id="tree-container">` inside the body of all the html files being used. 

Javascript functions: To load the visualization on the html file add the following functions to the webpage javascript code. 
```
PhyloDisplay(NEWICKpath,CSVpath,FASTApath) // will load the Treelink main visualization.
Clustree(NEWICKpath,Cut,CSVpath,FASTApath) // will load the Clustering visualization.
Phylogen(NEWICKpath,Cut,1,CSVpath) // will load the min graph visualization.
makemap(NEWICKpath,CSVpath) // will load the Treemap visualization. 
```
NEWICKpath refers to the location of the newick file, CSVpath to the location of the csv and FASTApath to the fasta file. Cut is the cutting value for the tree.
