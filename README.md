# Bilan Matthias (plan)

**Aim** = Analysis of nanopore (canine) (transcriptomic) data

**Methods**
  - *Manopore* : 
      - aim : QC and processing of nanopore reads  
      - method : 
        - nextflow
        - pipeline with different tools
      - results : 
        - [QC : nanocomp plots on DCS109, Number of reads, median length](http://tools.genouest.org/data/tderrien/igdrion/NanoComp-report-2020-07-24.html)
        - QC: mapping with minimaps (% reads mapped, unmapped...)
          - from Workman *et al.*: "The 360,000 unaligned pass reads had a median read length of 211 bases."
        - QC : [guppy versions impact on QC](https://gitlab.com/bioinfog/manopore/-/issues/11) 
        
  - *MacFab* : 
    - aim : 4 tools to reconstruct transcipt isoforms from nanopore
    - mehod :
      - snakemake
      - short description of the 4 methods
    - results 
      - Descriptive statistics
        - [per sample SQANTI](https://gitlab.com/bioinfog/macfab/uploads/f192cecb3e33a3e80784061088b6e2a8/bambu.CanFam3_sqanti_report.pdf)
        - comparing samples with [SQUANTI-like output](https://gitlab.com/bioinfog/macfab/uploads/0fc0052879deeaf683006e6a96232bd4/SQANTI_report.pdf). 
        - merging all fastq
          - nb of isoforms /genes 
          - knonwn vs novel isoforms/genes
          - number of 5' vs 3' extensions vs
      - RGASP-like comparison from macFab
      - [saturated plotversu num reads](https://gitlab.com/bioinfog/macfab/-/issues/10)
        - **at the gn and tx levels**
      - lncRNAs vs mRNA reconstruction : [RSEQC prelim analysis](https://gitlab.com/bioinfog/macfab/-/issues/13)
        - lncRNAs have a specific p[RT switching](https://www.sciencedirect.com/science/article/pii/S0888754305003770?via%3Dihub)
      
**Ccl/perspectives/ToDo list**
  - Manopore:
     - add new guppy versions (`bonito`)
  - MacFab 
     - new macfab methods ?
     - Transcript validation (TTS = CAGE ; TSS = tailFinder)  
  
*Notes*:
 - Focus on transcriptome reconstruction rather than quantification (no SIRVs)
 - Focus on lncRNAs reconstruction
 - Check talon vs bambu same number of isoforms
 - Check ORF annotation from SQANTI
  
      
    
