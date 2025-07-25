# Computational Practice: Perform a Basic Local Alignment Search Tool (BLAST) analysis at NCBI.

## Lab Overview
In this lab you will obtain a protein sequence from the human browser and find non-primate homologs in the protein databases.

## Lab Objectives:
In this lab, you will download BLAST a peptide sequence at NCBI and modify the output.
*	Obtain a peptide sequence from the UCSC genome browser.
*	Perform a BLAST analysis at NCBI.
*	Reformat BLAST hits into a hit table.

Follow these lab instructions:

### Task A: Obtain a peptide sequence from the UCSC genome browser.
Locate the STAT5A locus in the browser and then go to the gene information page for this transcript: ENST00000345506.8.  Find the 794 residue long FASTA sequence and save in a text file on the Linux desktop.  Name it something like this ‘LastName_FirstName_STAT5A.fasta’.

### Task B: BLAST the sequence against the NCBI nr database.  

#### Step 1 
After pasting the sequence in to the blastp algorithm at NCBI (https://blast.ncbi.nlm.nih.gov/), modify the BLASTP search as follows:
*	Exclude primates using Entrez limits (Primates (taxid:9443)) or the  “organism” field on the BLAST page.
*	Change the default E-value from 10 to 0.001. 
*	Use the BLOSUM45 scoring matrix.

#### Step 2 
Save the results as a ‘hit table’ in a plain text file. To do this, select all the sequences and click Download.  You can save as or comma delimited data.  This format is very useful for loading into Excel spreadsheets or data frames in Python/R/etc.
