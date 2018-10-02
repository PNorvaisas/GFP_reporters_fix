# GFP_reporters_fix
Reannotation of E. coli transcriptional reporter library (*Zaslaver et al. 2006*) based on most recent *E. coli* K-12 genome annotations
---
- Identification of promoter region amplicons in the most recent *E. coli* K-12 genome assembly and annotation based on primers provided in the original study using BLAST
- Identification of problematic amplicons and manual error-checking
- Cross-check with RegulonDB
- Linking of amplicons to promoters and their downstream genes
- Script - GFP_fix.py

## Files
- **GFP_fix.py** - Analysis script
- **Transcription_factors/** - Information from RegulonDB
- **Genome/** - *E. coli* K-12 genome files and BLAST prep

## GFP transcriptionalreporter library annotations
- **Info_Dharmacon.xlsx** - Library info from Dharmacon provider
- **Info_UAL.xls** - Library info from the paper (*Zaslaver et al. 2006*)
- **Joined.csv** - Clean info

## BLAST
- **UAL_primers.blast_input** - BLAST input file
- **UAL_primers_Ecoli_K12_MG1655_U00096.3.blast_output** - BLAST output file


## E. coli genome with mappings of various features
- **Ecoli_K12_MG1655_U00096.3_amplicons.gb** - *E. coli* K-12 genome sequence with amplicons
- **Ecoli_K12_MG1655_U00096.3_amplicons_TFBS.gb** - *E. coli* K-12 genome sequence with amplicons and TF binding sites
- **Ecoli_K12_MG1655_U00096.3_amplicons_TFBS_Prom.gb** - *E. coli* K-12 genome sequence with amplicons, TF binding sites (RegulonDB) and promoter regions (RegulonDB)
- **Ecoli_K12_MG1655_U00096.3_amplicons_TFBS_Prom_Operon.gb** - *E. coli* K-12 genome sequence with amplicons, TF binding sites (RegulonDB), promoter regions (RegulonDB) and operons (RegulonDB)

## Manual annotation of poorly defined/ambiguous amplicons
- **Gene_Operon_mapping_Ecoli_K12_MG1655_U00096.3.csv** - Feature-Amplicon matches
- **Gene_Operon_mapping_Ecoli_K12_MG1655_U00096.3_numbered.csv** - Feature-Amplicon matches
- **Gene_Operon_mapping_Ecoli_K12_MG1655_U00096.3_numbered_remove.csv** - Feature-Amplicon matches that need to be removed

## Results files
- **Amplicons_Ecoli_K12_MG1655_U00096.3.csv** - Promoter region amplicons based on primer sequences provided in *Zaslaver et al. 2006*
- **UAL_reannotated.csv** - All info
- **UAL_reannotated_multiple_reporting.csv** - All info with multiple gene reporting
- **UAL_reannotated_unique.csv** - All info with unique gene reporting

