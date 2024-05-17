## Ref mapping

- Ref mapping script
	### Essential: 
	- Input: ref.fa file_1.fq (file_2.fq) and output name

	- Processing: 
		- Clean the reads
		- Index the reference
		- Map the reads
	- Output: file.sam(bam)
 
	  
	### Desired: 
	- Check the input
	- Create a sam(bam) with mapped reads only
	- Generate mapping statistics
	- Generate the consensus sequence
	- Look for variants


	### Advanced:
	- Give the help message
	- Check whether the input files are in the right format
	- Give the option to choose the mapping program (bwa, bowtie2, tanoti, minimap2)
 	- Take program specific-parameters
	- Create the sam(bam) file with the same name as the input filename (with an appropriate file extension)
	- Check whether the reads are Illumina/ONT and run the analysis accordingly


## De novo assembly 

- De novo aasembly script
	### Essential: 
	- Input: file_1.fq (file_2.fq), output name

	- Processing: 
		- Clean the reads
    		- Create two directories for Spades and IDBA_UD outputs
		- Assemble using Spades and IDBA_UD
		- Use different k-mer sizes
    
	- Output: Assembled contigs
 
	  
	### Desired: 
	- Get the longest contig


	### Advanced:
	- Give the help message
	- Check the longest contigs orientation
	- Change the orientation if it is a reverse complement
	- Take program-specific parameters from the user
	- Use different de novo assemblers and combine the contigs to generate a super-contig