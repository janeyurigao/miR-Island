# miR-Island
an ultrafast and memory-efficient tool for plant miRNA annotation and expression analysis


INSTALLATION OF THIRD PARTY SOFTWARE

Note: To reduce time consuming, multiple threads specificity is applied in miR_Island. Your perl version must be equal to or greater than 5.10. You can check the perl version by running perl -v, and see if it is possible to use multiple threads by running perl -V and looking at the Platform section. If you have useithreads=define you can use the specificity.
Several dependencies are required to run miR_Island.
   
1: bowtie (used for aligning small RNA-seq to reference genome). The bowtie package can be downloaded from the site: http://sourceforge.net/projects/bowtie-bio/files/bowtie/. Our test version is 0.12.9.

2: samtools (tools for alignments in the SAM format). Samtools can be downloaded from the site: http://samtools.sourceforge.net/. Our test version is 0.1.19.

3: ViennaRNA (RNAfold is used for predicting hairpin structure). The Vienna RNA package is currently at http://www.tbi.univie.ac.at/RNA/.  Our test version is 2.0.0.

4: bioperl (used to improve the operation efficiency). Users are recommended to install bioperl according to http://www.bioperl.org/wiki/Installing_BioPerl. Our test version is 1.6.901.

5: Bio::DB::Sam (used to handle the SAM/BAM format alignment ). When you install Bio::DB::Sam module, you should depress the tar.gz of samtools and change directory to the depressed folder, then run "make CXXFLAGS=-fPIC CFLAGS=-fPIC CPPFLAGS=-fPIC". At last, you install Bio::DB::Sam module.

INSTALL MIR_ISLAND

Download the .tar.gz file from http://www.ncrna.net/tools/miR-island_v1.0.tar.gz and unpack. Then put the scripts into your PATH. This is done by typing the following lines:
echo 'export PATH=/path/to/miR_island:$PATH' >> ~/.bashrc
source ~/.bashrc
Note: "/path/to/miR_island" should be changed to the real location of miR_island folder.
You can test by typing miR_island.pl on the command line with no parameters. You should get a help message.

