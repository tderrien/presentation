# Bilan Matthias (plan)

**Aim** = Analysis of nanopore (canine) (transcriptomic) data

**Methods**
  - *Manopore* : 
      - aim : QC and processing of nanopore reads  
      - method : 
        - nextflow
        - pipeline with different tools
      - results : 
        - QC : nanocomp plots on DCS109, Number of reads, median length
        - QC: mapping with minimaps (% reads mapped, unmapped...)
        - QC : guppy versions impact on QC
        
  - *MacFab* : 
    - aim : 4 tools to reconstruct transcipt isoforms from nanopore
    - mehod :
      - snakemake
      - short description of the 4 methods
    - results 
      - nb of isoforms /genes 
      - knonwn vs novel isoforms/genes
      - saturated plot
      - lncRNAs vs mRNA reconstruction
      
**Ccl/perspectives/ToDo list**
  - Manopore:
     - add new guppy versions (`bonito`)
  - MacFab 
     - new macfab methods ?
     - Transcript validation (TTS = CAGE ; TSS = tailFinder)  
  
      
    
