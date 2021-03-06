<h2>Step 1: Get the tools</h2></b>
    The tools needed for this workflow are:<br>
    <b>Picard</b>: http://picard.sourceforge.net/<br>
    <b>Samtools</b>: http://samtools.sourceforge.net/<br>
    <b>Burrows-Wheeler Aligner</b>: http://bio-bwa.sourceforge.net/<br>
    <b>GATK</b>: https://www.broadinstitute.org/gatk/download<br>
    <b>Cuneiform</b>: https://github.com/joergen7/cuneiform
    
<h2>Step 2: Get the files</h2>
Reads: ftp://ftp.1000genomes.ebi.ac.uk/vol1/ftp/data/HG00096/sequence_read/<br> Known variants: ftp://ftp-trace.ncbi.nih.gov/1000genomes/ftp/release/20110521/ALL.chr22.phase1_release_v3.20101123.snps_indels_svs.genotypes.vcf.gz<br>
Training data: http://gatkforums.broadinstitute.org/discussion/1215/how-can-i-access-the-gsa-public-ftp-server
    
<h2>Step 3: Prepare the callers</h2>
Make the tools callable from your path. Picard and GATK need a bit of an extra handling.<br> GATK supports no Java 1.8 at the moment, if your standart version is 1.8, you need to call the GenomeAnalysisTK.jar with a prior version, best would be 1.7.<br> Create a bash script for picard, calling a jar in the form of: picard-tools-1.114/picard-tools-1.114/$1 <br> This will enable you to give the desired jar as first argument after the call.
    
<h2>Step 4</h2>
 Navigate to the folder where all the data-files are stored and start cuneiform there.

<h2>Step 5: Run the workflow.</h2>
<b>Good luck!</b>