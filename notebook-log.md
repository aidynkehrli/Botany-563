Final Project Data Set: Phylogeny of Gonioctena leaf beetles (Coleoptera; Chrysomelidae) 

"A phylogenetic analysis of the genus Gonioctena (Coleoptera, Chrysomelidae) based on allozyme data (17 loci) and mitochondrial DNA sequence data (three gene fragments, 1,391 sites) was performed to study the evolutionary history of host-plant shifts among these leaf beetles. This chrysomelid genus is characteristically associated with a high number of different plant families. The diverse molecular data gathered in this study are to a large extent congruent, and the analyses provide a well-supported phylogenetic hypothesis to address questions about the evolution of host-plant shifts in the genus Gonioctena. The most-parsimonious reconstruction of the ancestral host-plant associations, based on the estimated phylogeny, suggests that the Fabaceae was the ancestral host-plant family of the genus. Although most of the host-plant shifts (between different host species) in Gonioctena have occurred within the same plant family or within the same plant genus, at least eight shifts have occurred between hosts belonging to distantly related and chemically dissimilar plant families." The link to my data set is copied below: 
https://pubmed.ncbi.nlm.nih.gov/11975339/

I attemped to download miniconda (https://docs.conda.io/en/latest/miniconda.html), but was unable to initially. After a little while, I was able to install miniconda and use it to install ClusalW. Once miniconda was downloaded, I used the code "conda install -c bioconda clustalw" to install ClusalW. 

Additionally, I downloaded MAFFT (https://mafft.cbrc.jp/alignment/software/).

I copied and pasted the sequences for each gene marker (from my data) into a Visual Studio Code-3. This process took some time as my data set would not let me copy and paste every sequecne at the same time. When reproducing this project, I would take into account that this process takes a lot of time to complete. When I finished copying my data set completely, I saved each one as a text file. I saved each text file in my Botany-563 folder on my Desktop. I named each folder according to which marker they contained. I named the first text file "beetles-COII-data", the second file "beetles-12s-data", and the third file "beetles-16s-data." Remember to convert all of our data files into a .txt file. 

Then, I realized that the data sequences from my data set are already aligned, and that I did not need to realign them. From the article, I learned that the researchers aligned the data sequences with ClusalW, which I would have used as well if the data was not already aligned. 

I downloaded R studio and R using this link: https://posit.co/download/rstudio-desktop/. In R Studio, I installed the various packages by using the code "install.packages("adegenet", dep=TRUE)" and then using the code "install.packages("phangorn", dep=TRUE)". After installing the packages, I used the code "library(ape)", then  "library(adegenet)", and finally "library(phangorn)".

I tried to create a tree on R, but was unsuccessful. I got many errors when I used the code "dna <- fasta2DNAbin(file="beetles_COII_data.fasta")". If this code were successful, then you would use the code "D <- dist.dna(dna, model="TN93")", then you would use the code "tre <- nj(D)", then "tre <- ladderize(tre)", then "plot(tre, cex=.6)", anf finally "title("A simple NJ tree")". 

I downloaded iqtree using this link: http://www.iqtree.org/#download. I then ran the command "iqtree -s beetles_COII_data.fasta -bb 1000 -nt AUTO". To view the tree, run library(ape) in R. Then run myTree <- read.tree(file="Marker_42657_aligned_formated.fasta.iqtree") and plot(myTree) to view the ML tree. To select an outgroup, myTree <- root(myTree, outgroup="PB1D10") and plot(myTree)



