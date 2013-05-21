calc.dnds.pl :                         Calculates pairwise dn/ds ratios of all input sequences. Note: the sequences have to be alligned and in fasta format. In addition its assumed they start inframe. 

calc.gc.pl :                           Calculates the gc content of sequences in fasta format.

calc.kmerfreq.pl :                     Calculates kmer frequency in a set of input fasta sequences. The kmer length and minumim length of sequences can be changed.

extract.read2.using.read1.pl :         Extract read 2 using read 1 from two fasta files. Usefull when having a subset of read 1 and wanting the pairs extracted from the read 2 file.

mannotator.totab.add.pl :              Allows you to add more data points to a tab formated mannotator file. The extra data must be formatted as: contigid "tab" DATA1 "tab" DATA2.. Usefull to add e.g. coverage or binning information to all contigs.

mannotator.totab.pl :                  Converts the mannotator gff file into tab format (see the mannotator project). Also splits coulmns with multiple entries and arranges all unique entires in a column each. Identifies "=" as definition field and ; in the ontology field.

pandaseq.remove2bases.frombarcode.pl : Removes 2 bases from the barcode in fastq files. Used to circumvent the limitation in padaseq that assumes the header to be 6 bp long.

split.amphora.alignments.bin.pl :      Processes the .aln files output by Amphora2. The output needs to be fasta formatted and without reference sequences. The script creates stats on the number of genes and creates combined aligned files that can quickly be scanned through. In addition the program can split the results into different files based on an input bin file. The bin file needs to be in the format contigname "tab" bin. e.g. ">10	bin0". The header in the input alignments need to be in the format of e.g >10_whatever. The first "_" character is used to split the header of the input sequences. By using the -DNA feature of Amphora or FragGeneScan as orf predicter the header should be fine. 

split.assembly.bins.pl :               Splits a fastafile into multiple fastafiles based on an input bin file (format: fasta.header.name "tab" bin). 

splitpe.fasta.pl :                     Splits a combined paired end fasta file into two separate fasta files.

splitpe.fastq.pl :                     Splits a combined paired end fastq file into two separate fastq files.

template.pl :                          Nice perl template supplied by Mike Immelfort.
