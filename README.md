# Brower_rebuttal_Antenna_2025
Supplementary figures supporting the rebuttal in Antenna 2025.
These figures support our rebuttal of XXXX.

Figure 1: Maximum likelihood and maximum parsimony trees of the 26 kb section of the genome (Hmel218003:758703-784954) showing individual branches and accession numbers. Maximum likelihood tree based on chromosome 3.

Figure 2: Maximum likelihood analysis of a 26 kb section of the genome (Hmel218003:758703-784954) within the ~50 kb cis-regulatory region of the colour patterning gene optix. This is figure is identical to Figure 2 of our rebuttal in Antenna.

Whole genome sequences (fastq) were downloaded from Genbank, selecting individuals with the highest sequence coverage.
Fastq files were aligned to the Hmel2.5 reference genomes (Heliconius_melpomene_melpomene_Hmel2.5.scaffolds.fa) using bwa mem (BWA 0.7.17). 
The resulting sam/bam files were sorted and duplicates marked using samtools (SAMtools 1.20) and picard (picard 2.25.5). 
Genotyping was carried out using GATK 4.3.0 as follows: 
   1) GATK HaplotypeCaller was used on each bam file.
   2) GATK CombineGVCFs was used to combine individual GVCF files
   3) Genotyping using GATK GenotypeGVCFs.

From the VCF, a PHYLIP format sequence alignment for the genomic interval of interest was created using vcf2phylip

Bootstrapped maximum likelihood trees were generated from the alignments using IQ-TREE 2.3.5
Bootstrapped maximum parsimony trees were generated from the alignments using MPBoot 1.1.0
