Step 1: Get the files
    Reads: ftp://ftp.1000genomes.ebi.ac.uk/vol1/ftp/data/HG00096/sequence_read/
    Known variants: ftp://ftp-trace.ncbi.nih.gov/1000genomes/ftp/release/20110521/ALL.chr22.phase1_release_v3.20101123.snps_indels_svs.genotypes.vcf.gz
    Training data: http://gatkforums.broadinstitute.org/discussion/1215/how-can-i-access-the-gsa-public-ftp-server
    
Step 2: Edit the known variants, to match the contigs with the reference files
    For example for a file for chromosom 22:
    sed '/^22/s/22/chr22/' source.chr22.vcf > target.chr22.vcf
    
Step 3: Navigate to the folder where all the files are stored and start cuneiform there

Step 4: Run the workflow. Good luck!