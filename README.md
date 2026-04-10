# Analysis of LC morphologies

Data and notebooks for analysis of Locus Coeruleus (LC) single neuron morphologies. This repository contains notebooks for the generation of figures related to morphological analyses in Su et. al. 2026. These notebooks are also executable via reproducible run in CodeOcean.

__LC Manuscript Figure 2 Analyses__  
* Visualization of exemplar LC morphologies. These are 3d html renderings which can be manipulated and repositioned.  
* Brain-wide LC projections heatmap. This summary plot shows the projections of the reconstructed LC population to coarse CCF regions, quantified by axonal length. Axon and dendritic length/branching is also quantified relative to the LC population. Each column is one neuron, sorted by top projection target.  
* Correlation (spearman) matrix of LC projections and axon/dendrite features. Correlation between regions reflects the relationship between axon length in those regions.  
* Analysis of spatial organization of LC morphologies. Axons are colored by the corresponding soma's dorsal/ventral position in LC. This is a 3d html rendering which can be manipulated and repositioned (large file size may require downloading and re-opening in a web browser).  
* Spatial organization of top projection targets. Soma positions in LC are colored by the CCF region to which they send the most axon length.  
  
__LC Manuscript Supplemental Figure A4 Analyses__  
* Comparison of LC axon length / branching against MouseLight dataset. Fully traced LC morphologies are colored dark purple, while incomplete reconstructions (cells with projections that are cut off from samples missing spinal cord) are colored light purple.  
* Projection coverage of cortical regions. Flatmap representations of the fraction of cortically projecting LC neurons innervating a given cortical area, and the per neuron axon density (axon length / neurons / areal volume).  
* Correlation matrix of LC projections to cortical areas. Spearman correlation of axonal length in different cortical areas, sorted by hierarchical clustering.  
* Correlation of LC projections to different cortical areas. Flatmap representations of spearman correlation to example seed regions (e.g. MOs, VISp). Equivalent to slices of the correlation matrix.
* Correlation between cortical areas as a function of distance between the regions (computed from volume centroid).  
* Correlation matrix of LC projections to cortex and cerebellum. Spearman correlation of axonal length, from neurons with projections to cortex and/or cerebellum.  
  
  
Neuron reconstructions are additionally available on the Neural Dynamics morphology portal:  
https://morphology.allenneuraldynamics.org/

CodeOcean release version:  
https://codeocean.allenneuraldynamics.org/capsule/5888750/tree

Github Repo:  
https://github.com/AllenNeuralDynamics/aind-LC-morphologies