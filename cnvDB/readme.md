# [XXX_FULL_NAME_XXX](xxx)

The [XXX_SHORT_NAME_XXX](xxx) is a crowdsourcing initiative to provide information about **C**opy **N**umber **V**ariations of the Spanish population to the scientific/medical community. We accept submissions from WES or WGS, no matter whether these come from healthy or diseased individuals.

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

* [Browser panel](#browser_panel) (Fig1.A). Consists on an embedded [Integrative Genomics Viewer](https://igv.org/) preloaded with the Spanish CNV database and some others useful tracks. 
* [Search and selection panel](#search_panel) (Fig1.B). Provides several filters for specifying the genomic region and the data to be shown.
* [Filtering status panel](#filtering_panel) (Fig1.C). Shows information about the active filters.

![alt web interface][fig1]


### <a name="browser_panel">Browser panel</a>
[IGV](https://igv.org/) provides several navigation controls for specifying the genomic region to view. A ruler indicating the extent of the current region is displayed below the toolbar, and the size of the region and its genomic coordinates are displayed in the toolbar.

* **Select a chromosome**. The chromosome dropdown menu in the toolbar (Fig1.A.1) includes an entry for every chromosome or contig in the reference genome. Selecting a chromosome from the menu will set the view to include the whole chromosome. The ruler also includes a cytoband ideogram.
* **Enter genomic coordinates**. In the text box where the genomic coordinates are displayed (Fig1.A.2), you can type the coordinates of the region you want to view (e.g. chr17:41,195,312-41,278,500). The thousands separator is optional, but the chromosome name is required.
* **Search by gene name**. In the text box where the genomic coordinates are displayed (Fig1.A.2), type the name of a gene (e.g. BRCA1) and hit return or click on the magnifying glass. IGV will look up the genomic coordinates for that gene and set the viewing region accordingly.
* **Spanish CNVs database**. The _CNVs_ track (Fig1.A.3) displays Copy Number Variations that fulfill the filtering criteria (Fig1.C). Clicking on each element displays additional information (see [XXX](xxx)).
* **World populations CNVs**. _CNVs_ derived from [gnomad](https://gnomad.broadinstitute.org/) and [1000 genomes project](https://www.internationalgenome.org/) are provided as two additional tracks (Fig1.A.4). Frequencies for multiallelic CNVs (MCNV) are sumarized in _deletions_ (CN0 and CN1) and _duplications_ (CN3 or more)
* **Regularoty regions**. The regulatory region track (Fig1.A.5) includes _protomoters_, _enhancers_, _transcription factor binding sites_, _CTCF binding sites_ and _open chromatine regions_ as described in [UCSC](hgdownload.soe.ucsc.edu). 
* **Clinvar structural variants**. This track (Fig1.A.6) contains known clinical relevant _Copy number gain_, _copy number loss_, _duplication_ and _deletion_ from [clinvar](https://www.ncbi.nlm.nih.gov/clinvar/).



### <a name="search_panel">Search panel</a>
This section controls the CNVs displayed in the _CNVs_ track. By default, the whole dataset is displayed.

* **Variant type**. Use this filter to show _deletions_, _duplications_ or both types of CNVs.
* **Annotation**. CNVs are annotated with different databases (see [XXX](xxx)). Select the annotations you are interest in (e.g. DisGeNET) and type some words to see suggestions. Use the plus button to append the filter. Multiple filters are allowed.
* **Frequency**. CNVs frecuency are calculated as the ratio of individuals having at least one CNV overlapping it. 
* **Samples**. Despite gene pleiotropy cannot be completely ruled out, samples were binned at higher disease ICD10 categories. The main objetive is using the repository as a pseudo-control population for finding new disease-causing CNVs, with the idea that ‘disease A is a healthy control for disease B’.

### <a name="filtering_panel">Filtering status panel</a>
The filtering status section (Fig1.C) provides a summary of the filters applied to the CNV database. By default, the whole database is shown. Use the search panel (Fig1.B) to add or remove filters.


## <a name="annotations">CNV annotations</a>

<!---
DisGeNET	7.0, January 2020
GO	2021-02-01
PHENOTYPE	Generated: 14-abr-2021
Clinvar	2021-04-18
DOSE	20 January 2021
OMIM	Generated: 2021-04-19
ORPHANET	1.3.7 \/ 4.1. ,2021-04-01
Mappability Consensus	2011-05-04
-->


## <a name="citation">Citation</a>







[fig1]: img/fig1.svg "Web interface"













