# BIOC3301-QIIME-Scripts

This GitHub Repository contains all the QIIME scripts required to replicate our analysis as described in the main text. The scripts are utilised in the same order as seen in the Materials/Methods and Results sections. Below is a summary of what process each script performs. Further details and help are available here: http://qiime.org/scripts/. Our mapping file (map.tsv) is also included and is adjusted accordingly.

CDA - AB and PB : Performs core_diversity_analyses.py on .biom table containing OTUs within the Acidobacteria (AB) and Proteobacteria (PB) phyla only.

Compare Alpha Diversity : Performs compare_alpha_diversity.py statistical analysis on rarefaction plots produced from CDA (Core Diversity Analses).

Compare Categories (ANOSIM) : Performs compare_categories.py to assess statistical significance of beta-diversity PCoA plots.

Core Diversity Analyses (CDA) : Performs core_diversity analyses.py on .biom table containing all identified OTUs. Contains subscripts: alpha_rarefaction.py, beta_diversity_through_plots.py, summarize_taxa_through_plots.py. Also contains  non-workflow scripts make_distance_boxplots.py, compare_alpha_diversity.py, and group_significance.py.

Filter OTUs by sample : Performs filter_samples_from_otu_table.py to remove specific samples from .biom table using a manually altered mapping file.

Filter OTUs by taxa : Performs filter_taxa_from_otu_table.py  to isolate the AB and PB phyla from .biom table. 

Group Significance (All) : These three scripts compare OTU frequencies across sample groups, performed three times to analyse three different levels of taxonomy. (group_significance.py).

Join Paired Ends : Performs join_paired_ends.py to join paired-end Illumina reads.

Make OTU heatmap : Performs make_otu_heatmap.py to plot heatmap of OTUs of classes under the AB and PB phyla.

Pick OTUs : Performs pick_closed_reference_otus.py to construct an OTU table (.biom) from a closed reference.

Split Libraries : Performs split_libraries_fastq.py to demultiplexing of fastq format sequences.

