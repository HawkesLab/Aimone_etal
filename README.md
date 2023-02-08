## Aimone CD, Giauque H, Hawkes CV. Fungal symbionts generate water-saver and water-spender plant drought strategies via diverse effects on host gene expression.


## Supplementary Data and Analysis
Data and analyses associated with this project.


## Author Contact Information
Christine Hawkes	
112 Derieux Place, Thomas Hall, North Carolina State University, Raleigh, NC 27607
chawkes@ncsu.edu

## Experiment description
Panicum hallii var hallii HAL2 plants were inoculated individually with six foliar fungal endophytes or fungus free controls and subjected to 5% or 20% soil moisture treatments. The fungi were selected for their previously observed effects on plant drought physiology, inducing either a “water saver” or a “water spender” strategy in the host. Plants were grown in enclosed microcosms to prevent cross-contamination and each treatment and control included 6 replicates. All fungi were Ascomycetes isolated from plants in central Texas. Plants were monitored for height, wilt, water loss, and survival. At the harvest, we also measured oven-dried shoot and root biomass, and leaf colonization by the fungi (each on n=3 replicates). A subset of leaf replicates were further characterized by untargeted metabolomics profiling.

## File list  
### Data  
RNAseqPlantRespData.csv  
All_DEGs_log2fc.csv  
DEGs.txt  
FPKM_replicates.csv  
FPKM_sampledata.csv  

### Scripts and analyses  
TXRNAseq_Permanovas.pdf  
TXRNAseq_PCoA.pdf  
TXRNAseq_Lasso.pdf  
GeneFile_TRT_CON_DEGs_trimmed.xlsx  
TRT_CON_biograph_96.txt  

## File descriptions  
### Data  

RNAseq_PlantRespData.csv – All plant response data used for permANOVAs. Includes the following measurements:   
rgr	= Relative height growth rate (mm/d)    
wilt = Days to first wilt (d)  
death	= Days to first tiller death (survival)	(d)  
waterloss	= Rate of plant water loss	(g/d)  
totbiom	= Combined shoot and root dry biomass	(g)  
leafcol	= proporation of eaf colonization by fungi

All_DEGs_log2fc.csv – log2 fold-change data calculated on raw gene expression data plus one to avoid issues with zero values. All genes that were differentially expressed in at least one treatment are included for use in LASSO regression.  

DEGs.txt – List of genes that were differentially expressed in at least one treatment for use in pruning full dataset for PCoA.   

FPKM_replicates.csv – Raw replicate-level gene expression data output from TuxOP used in fragments per kilobase of exon per million mapped fragments. Used in PCoA analysis.   

FPKM_sampledata.csv – Treatment data associated with the FPKM_replicates.csv for use in graphing the PCoA results.  

### Scripts and analyses   
TXRNAseq_Permanovas.pdf – knitted R markdown script for permANOVAs of plant responses as a function of treatments. Correlations among the plant responses are also included here.  

TXRNAseq_PCoA.pdf – knitted R markdown script for ordination analysis of all plant genes and differentially expressed genes.  

TXRNAseq_Lasso.pdf – knitted R markdown script for LASSO regression analysis of plant responses as a function of plant genes that were differentially expressed in at least one treatment.  

GeneFile_TRT_CON_DEGs_trimmed.xlsx – gene list output from RTP-STAR trimmed to only those genes present in > 95% of iterations. TRT = treatment and CON = control. Fungal treatments are indicated by the first three letters (CER = Cercospora, COC = Cochliobolus, NIG = Nigrospora, PEN = Penicillium, SOR = Sordaria) and water treatments by the fourth letter (D = drought, W = well-watered). Used for visualizing networks in Cytoscape.  

TRT_CON_biograph_96.txt – predicted regulatory interactions output from RTP-STAR trimmed to only those genes present in > 95% of iterations. TRT = treatment and CON = control. Fungal treatments are indicated by the first three letters (CER = Cercospora, COC = Cochliobolus, NIG = Nigrospora, PEN = Penicillium, SOR = Sordaria) and water treatments by the fourth letter (D = drought, W = well-watered). Used for visualizing networks in Cytoscape.  


## Note  
Data files must be placed in your working directory for the analyses, or paths must be specified.  

## Publication information  
A manuscript based on these data is currently in review. This section will be updated as appropriate.  

## Funding information  
This work was supported by the USDA National Institute of Food and Agriculture Physiology of Agricultural Plants program (grant no. 2017-67013-29207), USDA Hatch (accession no. 1018688), NSF Plant Genome Research Program (IOS-0922457), and the Texas Ecolab program.   

## Additional data – raw sequences  
Sequence data are available at the NCBI Sequence Read Archive (PRJNA777108).  
