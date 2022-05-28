#Celem projektu była analiza SNP 


1. First, I took 1,000,000 readings from each sample using the fastq-dump command.
2. The next step was the qualitative analysis of the given readings, for this we used fastqc because the quality readings were approx.
So I deleted only those readings that were beyond quality with the trimmomatic, then tested the quality again and showed the results in the Data folder.
3. Then I downloaded the reference genome and prepared the annotation library with hisat2-buildindex.
4. After mapping to the ref genome, I changed the data from SAM files to BAM files using samtools tools.
5. Next step was remove duplicates and split data. I use here gatk tools.
6. I used Bcftools to detect variants and the result was a vcf file.
7. The obtained data can be visualized by using the vcfR package and the IGV program
