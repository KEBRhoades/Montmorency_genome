By and large I followed the tutorial created by Kamil Jaron for his oh-know workshop: https://github.com/KamilSJaron/oh-know/wiki/Separate-sub-genomes-of-an-allopolyploid

With a few exceptions:  
* I ran jellyfish 2.2.10 in a conda environment  
* Rather than using a loop to separate the genome fasta into individual chromosome files I used seqtk (also within a conda environment)  
  *  seqtk: https://github.com/lh3/seqtk  
  *  (I couldn't get that one loop to work I don't know why)  
* Counted 25mers based on the success of 25mer spectra in genome assembly steps
* In the 'jellyfish dump' step, retained all 25mers present more than 10x per chromosome  

Then downloaded all dumps.col files to my computer for analysis in R.
