# [XXX_FULL_NAME_XXX](xxx)
![alt logo][logo]


[XXX_SHORT_NAME_XXX](xxx) is a crowdsourcing initiative to provide information about **C**opy **N**umber **V**ariations of the Spanish population to the scientific/medical community. We accept submissions from WES or WGS, no matter whether these come from healthy or diseased individuals.

The sequences were contributed by different consortiums and projects, including groups from the Spanish Network for Research in Rare Diseases, [CIBERER](https://www.ciberer.es/), results from the [EnoD](https: //www.ciberer.es/en/transversal-programmes/scientific- projects/undiagnosed-rare-diseases-programme-enod), the [Project Genome 1000 Navarra](https://www.nagen1000navarra.es/en) and other research groups and initiatives across Spain. 

[XXX_SHORT_NAME_XXX](xxx) is an open resource available at [http://csvs.clinbioinfosspa.es/cnv](http://csvs.clinbioinfosspa.es/cnv)


## <a name="TOC">Table of content</a>
 1. [Web interface](#interface)
    1. [Overview](#interface_overview)
    1. [Search panel](#interface_search)
    1. [Filtering status panel](#interface_filter)
 1. [CNV annotations](#annotations)
 1. [Citation](#citation)


## <a name="interface">Web interface</a>
The web interface has 3 main sections: 

* [Browser panel](#browser_panel) (Fig1.A). Consists on an embedded [Integrative Genomics Viewer](https://igv.org/) preloaded with the Spanish CNV database and some other useful tracks. 
* [Search and selection panel](#search_panel) (Fig1.B). Provides several filters for specifying the genomic region and the data to be shown.
* [Filtering status panel](#filtering_panel) (Fig1.C). Shows information about the active filters.

![alt web interface][fig1]


### <a name="browser_panel">Browser panel</a>
[IGV](https://igv.org/) provides several navigation controls for specifying the genomic region to view. A ruler indicating the extent of the current region is displayed below the toolbar, and the size of the region and its genomic coordinates are displayed in the toolbar.

* **Select a chromosome**. The chromosome dropdown menu in the toolbar (Fig1.A.1) includes an entry for every chromosome or contig in the reference genome. Selecting a chromosome from the menu will set the view to include the whole chromosome. The ruler also includes a cytoband ideogram.
* **Enter genomic coordinates**. In the text box where the genomic coordinates are displayed (Fig1.A.2), you can type the coordinates of the region you want to view (e.g. chr17:41,195,312-41,278,500). The thousands separator is optional, but the chromosome name is required.
* **Search by gene name**. In the text box where the genomic coordinates are displayed (Fig1.A.2), type the name of a gene (e.g. BRCA1) and hit return or click on the magnifying glass. IGV will look up the genomic coordinates for that gene and set the viewing region accordingly.
* **Spanish CNVs database**. The _CNVs_ track (Fig1.A.3) displays Copy Number Variations that fulfill the filtering criteria (Fig1.C). Click on an element to display additional information (see [CNV annotations](#annotations)).
* **World populations CNVs**. _CNVs_ derived from [gnomad](https://gnomad.broadinstitute.org/) and [1000 genomes](https://www.internationalgenome.org/) projects are provided as two additional tracks (Fig1.A.4). Frequencies for multiallelic CNVs (MCNV) are sumarized in _deletions_ (CN0 and CN1) and _duplications_ (CN3 or more)
* **Regularoty regions**. The regulatory region track (Fig1.A.5) includes _protomoters_, _enhancers_, _transcription factor binding sites_, _CTCF binding sites_ and _open chromatine regions_ as described in [UCSC](hgdownload.soe.ucsc.edu). 
* **Clinvar structural variants**. This track (Fig1.A.6) contains known clinical relevant _Copy number gain_, _copy number loss_, _duplication_ and _deletion_ from [clinvar](https://www.ncbi.nlm.nih.gov/clinvar/).



### <a name="search_panel">Search panel</a>
This section controls the CNVs displayed in the _CNVs_ track. By default, the whole dataset is displayed.

* **Genomic locus**. You can type a specific locus or a gene to find and show a given genomic region.  
* **Variant type**. Use this filter to show _deletions_, _duplications_ or both types of CNVs.
* **Annotation**. CNVs are annotated with different databases (see [CNV annotations](#annotations)). Select the annotations you are interest in (e.g. DisGeNET) and type some words to see suggestions. Use the plus button to append the filter. Multiple filters are allowed.
* **Frequency**. CNVs frecuency are calculated as the ratio of individuals having at least one CNV overlapping it. 
* **Samples**. Despite gene pleiotropy cannot be completely ruled out, samples were binned at higher disease ICD10 categories. The main objetive is using the repository as a pseudo-control population for finding new disease-causing CNVs, with the idea that ‘disease A is a healthy control for disease B’. Additionally, samples can also be filtered out according to their main [HPO](https://hpo.jax.org/app/).

### <a name="filtering_panel">Filtering status panel</a>
The filtering status section (Fig1.C) provides a summary of the filters applied to the CNV database. By default, the whole database is shown. Use the search panel (Fig1.B) to add or remove filters.


## <a name="annotations">CNV annotations</a>
We provide and extensive annotation of CNVs with clinical relevant databases. A CNV is annotated with some specific genomic region feature if overlapped. 

* **Gene Ontology Annotation (GOA)**. The [GOA](https://www.ebi.ac.uk/GOA/index) program aims to provide high-quality [Gene Ontology](http://geneontology.org/) (GO) annotations to proteins in the UniProt Knowledgebase (UniProtKB), RNA molecules from RNACentral and protein complexes from the Complex Portal.  GOA files contain a mixture of manual annotation and computationally assigned GO terms describing gene products.
* **Clinvar database**. [ClinVar](https://www.ncbi.nlm.nih.gov/clinvar/) is a freely accessible, public archive of reports of the relationships among human variations and phenotypes, with supporting evidence. It also provides gene-disease relationships.
* **DisGeNET**. [DisGeNET](https://www.disgenet.org/) is a discovery platform containing a collections of genes and variants associated to human diseases. DisGeNET integrates data from expert curated repositories, GWAS catalogues, animal models and the scientific literature.
* **Clingen**. [ClinGen](https://www.clinicalgenome.org/) is a National Institutes of Health (NIH)-funded resource dedicated to building a central resource that defines the clinical relevance of genes and variants for use in precision medicine and research. It provides a curated gene dosage sensitivity database.
* **The Human Phenotype Ontology**. The Human Phenotype Ontology [HPO](https://hpo.jax.org/app/) provides a standardized vocabulary of phenotypic abnormalities encountered in human disease. We provide HPO annotations derived directly from gene-phenotipe links and from the patient network analysis carried out by [A. Reyes-Palomares et at](https://doi.org/10.1186/s12864-016-2569-6).
* **Mappability**. The wgEncodeEH000322 track from [UCSC](hgdownload.soe.ucsc.edu) provides information about the mappability of the genome. This annotation can be useful to detect false positives and biases in CNV prediction software.
* 


## <a name="citation">Citation</a>
By downloading data from the Spanish CNV DataBase you accept the obligation of acknowledge its use in any publication, presentation, conference, poster or any public event in which you present results obtained in any way using the data downloaded.

To acknowledge the use of Spanish CNV Database data use a sentence similar to this one: “These results were obtained using Spanish CNV DataBase data ( http://csvs.babelomics.org/cnv)".

<!-- and in any publication you must cite the reference:-->






[fig1]: img/fig1.svg "Web interface"
[logo]: img/logo.svg "logo"














