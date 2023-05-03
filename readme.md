CODE USED TO CREATE R TREES AND MAXIMUM LIKELIHOOD TREES ON IQ TREE:

Last login: Wed Apr 26 16:28:11 on ttys001
(base) aidynkehrli@Aidyns-MacBook-Pro ~ % 
(base) aidynkehrli@Aidyns-MacBook-Pro ~ % pwd
/Users/aidynkehrli
(base) aidynkehrli@Aidyns-MacBook-Pro ~ % cd Desktop/Botany-563 
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   .DS_Store

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	3-30-homework-test.model
	Terminal Saved Output.txt
	beetles_12s_data.fasta.txt
	beetles_16s_data.fasta.txt
	beetles_COII_data.fasta.txt
	iqtree-1.6.12-MacOSX/

no changes added to commit (use "git add" and/or "git commit -a")
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git branch
* master
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   .DS_Store

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	3-30-homework-test.model
	Terminal Saved Output.txt
	beetles_12s_data.fasta.txt
	beetles_16s_data.fasta.txt
	beetles_COII_data.fasta.txt
	iqtree-1.6.12-MacOSX/

no changes added to commit (use "git add" and/or "git commit -a")
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git pull
remote: Enumerating objects: 43, done.
remote: Counting objects: 100% (43/43), done.
remote: Compressing objects: 100% (39/39), done.
remote: Total 43 (delta 19), reused 2 (delta 1), pack-reused 0
Unpacking objects: 100% (43/43), 11.95 KiB | 313.00 KiB/s, done.
From https://github.com/aidynkehrli/Botany-563
 * [new branch]      main       -> origin/main
Already up to date.
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git add .
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git commit -m "updated files"
[master 6462549] updated files
 Committer: Aidyn Kehrli <aidynkehrli@Aidyns-MacBook-Pro.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 13 files changed, 20393 insertions(+)
 create mode 100644 3-30-homework-test.model
 create mode 100644 Terminal Saved Output.txt
 create mode 100644 beetles_12s_data.fasta.txt
 create mode 100644 beetles_16s_data.fasta.txt
 create mode 100644 beetles_COII_data.fasta.txt
 create mode 100644 iqtree-1.6.12-MacOSX/.DS_Store
 create mode 100644 iqtree-1.6.12-MacOSX/beetles_COII_data.fasta.log
 create mode 100755 iqtree-1.6.12-MacOSX/bin/iqtree
 create mode 100644 iqtree-1.6.12-MacOSX/example.cf
 create mode 100644 iqtree-1.6.12-MacOSX/example.nex
 create mode 100644 iqtree-1.6.12-MacOSX/example.phy
 create mode 100644 iqtree-1.6.12-MacOSX/models.nex
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git push
Enumerating objects: 19, done.
Counting objects: 100% (19/19), done.
Delta compression using up to 8 threads
Compressing objects: 100% (16/16), done.
Writing objects: 100% (17/17), 2.87 MiB | 4.16 MiB/s, done.
Total 17 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/aidynkehrli/Botany-563.git
   c602cbe..6462549  master -> master
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git branch
* master
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % cd ..
(base) aidynkehrli@Aidyns-MacBook-Pro Desktop % pwd
/Users/aidynkehrli/Desktop
(base) aidynkehrli@Aidyns-MacBook-Pro Desktop % mkdir tmp
(base) aidynkehrli@Aidyns-MacBook-Pro Desktop % cd tmp 
(base) aidynkehrli@Aidyns-MacBook-Pro tmp % git clone https://github.com/aidynkehrli/Botany-563.git
Cloning into 'Botany-563'...
remote: Enumerating objects: 73, done.
remote: Counting objects: 100% (73/73), done.
remote: Compressing objects: 100% (64/64), done.
remote: Total 73 (delta 25), reused 29 (delta 4), pack-reused 0
Receiving objects: 100% (73/73), 2.90 MiB | 5.11 MiB/s, done.
Resolving deltas: 100% (25/25), done.
(base) aidynkehrli@Aidyns-MacBook-Pro tmp % cd ..
(base) aidynkehrli@Aidyns-MacBook-Pro Desktop % cd Botany-563 
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	Analysis/
	Data/
	Figures/
	data_clean/
	data_raw/
	notebook-log.md

nothing added to commit but untracked files present (use "git add" to track)
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git add .
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git commit -m "added main files and folders"
[master 7ff78cf] added main files and folders
 Committer: Aidyn Kehrli <aidynkehrli@Aidyns-MacBook-Pro.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 7 files changed, 28 insertions(+)
 create mode 100644 Analysis/README.md
 create mode 100644 Data/README.md
 create mode 100644 Data/beetle_data
 create mode 100644 Figures/README.md
 create mode 100644 data_clean/README.md
 create mode 100644 data_raw/README.md
 create mode 100644 notebook-log.md
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % pwd
/Users/aidynkehrli/Desktop/Botany-563
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git push
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 8 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (7/7), 2.42 KiB | 2.42 MiB/s, done.
Total 7 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/aidynkehrli/Botany-563.git
   6462549..7ff78cf  master -> master
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   .DS_Store
	deleted:    beetles_12s_data.fasta.txt
	deleted:    beetles_16s_data.fasta.txt
	deleted:    beetles_COII_data.fasta.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	.RData
	.Rapp.history
	.Rhistory
	R Console.txt
	R_tree_12s_data.pdf
	R_tree_16s_data.pdf
	R_tree_COII_data.pdf
	beetles_12s_data.fasta
	beetles_16s_data.fasta
	beetles_COII_data.fasta
	beetles_COII_data2.fasta

no changes added to commit (use "git add" and/or "git commit -a")
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git add .
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git commit -m "updated files and folders"
[master 7d3491c] updated files and folders
 Committer: Aidyn Kehrli <aidynkehrli@Aidyns-MacBook-Pro.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 15 files changed, 1444 insertions(+), 361 deletions(-)
 create mode 100644 .RData
 create mode 100644 .Rapp.history
 create mode 100644 .Rhistory
 create mode 100644 R Console.txt
 create mode 100644 R_tree_12s_data.pdf
 create mode 100644 R_tree_16s_data.pdf
 create mode 100644 R_tree_COII_data.pdf
 create mode 100644 beetles_12s_data.fasta
 delete mode 100644 beetles_12s_data.fasta.txt
 create mode 100644 beetles_16s_data.fasta
 delete mode 100644 beetles_16s_data.fasta.txt
 create mode 100644 beetles_COII_data.fasta
 delete mode 100644 beetles_COII_data.fasta.txt
 create mode 100644 beetles_COII_data2.fasta
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git push
Enumerating objects: 15, done.
Counting objects: 100% (15/15), done.
Delta compression using up to 8 threads
Compressing objects: 100% (13/13), done.
Writing objects: 100% (13/13), 57.02 KiB | 7.13 MiB/s, done.
Total 13 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), completed with 2 local objects.
To https://github.com/aidynkehrli/Botany-563.git
   7ff78cf..7d3491c  master -> master
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % iqtree
zsh: command not found: iqtree
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % pwd
/Users/aidynkehrli/Desktop/Botany-563
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % cd iqtree-1.6.12-MacOSX 
(base) aidynkehrli@Aidyns-MacBook-Pro iqtree-1.6.12-MacOSX % ls
beetles_COII_data.fasta.log	example.cf			example.phy
bin				example.nex			models.nex
(base) aidynkehrli@Aidyns-MacBook-Pro iqtree-1.6.12-MacOSX % cd bin 
(base) aidynkehrli@Aidyns-MacBook-Pro bin % ls
iqtree
(base) aidynkehrli@Aidyns-MacBook-Pro bin % iqtree
zsh: command not found: iqtree
(base) aidynkehrli@Aidyns-MacBook-Pro bin % ./iqtree
IQ-TREE multicore version 1.6.12 for Mac OS X 64-bit built Aug 15 2019
Developed by Bui Quang Minh, Nguyen Lam Tung, Olga Chernomor,
Heiko Schmidt, Dominik Schrempf, Michael Woodhams.

Command-line examples (replace 'iqtree ...' by actual path to executable):

1. Infer maximum-likelihood tree from a sequence alignment (example.phy)
   with the best-fit model automatically selected by ModelFinder:
     iqtree -s example.phy

2. Perform ModelFinder without subsequent tree inference:
     iqtree -s example.phy -m MF
   (use '-m TEST' to resemble jModelTest/ProtTest)

3. Combine ModelFinder, tree search, ultrafast bootstrap and SH-aLRT test:
     iqtree -s example.phy -alrt 1000 -bb 1000

4. Perform edge-linked proportional partition model (example.nex):
     iqtree -s example.phy -spp example.nex
   (replace '-spp' by '-sp' for edge-unlinked model)

5. Find best partition scheme by possibly merging partitions:
     iqtree -s example.phy -sp example.nex -m MF+MERGE
   (use '-m TESTMERGEONLY' to resemble PartitionFinder)

6. Find best partition scheme followed by tree inference and bootstrap:
     iqtree -s example.phy -spp example.nex -m MFP+MERGE -bb 1000

7. Use 4 CPU cores to speed up computation: add '-nt 4' option

---
PoMo command-line examples:
1. Standard tree inference (HKY model, empirical nucleotide frequencies):
     iqtree -s counts_file.cf -m HKY+P

2. Set virtual population size to 15:
     iqtree -s counts_file.cf -m HKY+P+N15

3. Use GTR model and estimate state frequencies with maxmimum lilelihood:
     iqtree -s counts_file.cf -m GTR+P+FO

4. Polymorphism-aware mixture model with N=5 and weighted binomial sampling:
     iqtree -s counts_file.cf -m "MIX{HKY+P{EMP},JC+P}+N5+WB"

---
To show all available options: run 'iqtree -h'

Have a look at the tutorial and manual for more information:
     http://www.iqtree.org

(base) aidynkehrli@Aidyns-MacBook-Pro bin % pwd
/Users/aidynkehrli/Desktop/Botany-563/iqtree-1.6.12-MacOSX/bin
(base) aidynkehrli@Aidyns-MacBook-Pro bin % pwd
/Users/aidynkehrli/Desktop/Botany-563/iqtree-1.6.12-MacOSX/bin
(base) aidynkehrli@Aidyns-MacBook-Pro bin % cd ..
(base) aidynkehrli@Aidyns-MacBook-Pro iqtree-1.6.12-MacOSX % cd ..
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % ls
3-30-homework-test		Analysis			beetles_COII_data.fasta
3-30-homework-test.bionj	Data				beetles_COII_data2.fasta
3-30-homework-test.ckp.gz	Figures				data_clean
3-30-homework-test.iqtree	R Console.txt			data_raw
3-30-homework-test.log		R_tree_12s_data.pdf		iqtree
3-30-homework-test.mldist	R_tree_16s_data.pdf		iqtree-1.6.12-MacOSX
3-30-homework-test.model	R_tree_COII_data.pdf		notebook-log.md
3-30-homework-test.model.gz	Terminal Saved Output.txt	readme.md
3-30-homework-test.treefile	beetles_12s_data.fasta
30 Homework Test		beetles_16s_data.fasta
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % ./iqtree -s beetles_COII_data.fasta -bb 1000 -nt AUTO
IQ-TREE multicore version 1.6.12 for Mac OS X 64-bit built Aug 15 2019
Developed by Bui Quang Minh, Nguyen Lam Tung, Olga Chernomor,
Heiko Schmidt, Dominik Schrempf, Michael Woodhams.

Host:    Aidyns-MacBook-Pro.local (SSE4.2, 8 GB RAM)
Command: ./iqtree -s beetles_COII_data.fasta -bb 1000 -nt AUTO
Seed:    219955 (Using SPRNG - Scalable Parallel Random Number Generator)
Time:    Tue May  2 13:54:21 2023
Kernel:  SSE2 - auto-detect threads (8 CPU cores detected)

Reading alignment file beetles_COII_data.fasta ... Fasta format detected
Alignment most likely contains DNA/RNA sequences
Alignment has 20 sequences with 553 columns, 204 distinct patterns
150 parsimony-informative, 78 singleton sites, 325 constant sites
                     Gap/Ambiguity  Composition  p-value
   1  G_viminalis_1          0.00%    passed     92.35%
   2  G_Olivacea_1           0.00%    passed     96.73%
   3  G_rufipes              0.00%    passed     99.43%
   4  G_linnaeana            0.00%    passed     95.71%
   5  G_variabilis_1         0.00%    passed     76.03%
   6  G_fornicata            0.00%    passed     82.96%
   7  G_occidentalis         0.00%    passed     97.66%
   8  G_interposita_1        0.18%    passed     87.80%
   9  G_interposita_2        0.00%    passed     98.34%
  10  G_intermedia           0.00%    passed     93.85%
  11  G_quinquepunctata_2    0.00%    passed     89.19%
  12  G_holdausi             0.00%    passed     90.36%
  13  G_pallida_2            0.36%    passed     98.00%
  14  G_pallida_3            1.27%    passed     95.24%
  15  G_tredecimmaculata     0.00%    passed     86.21%
  16  G_nigropiagiata        0.00%    passed     95.29%
  17  G_kamikawai            0.00%    passed     96.12%
  18  G_rubripennis          0.00%    passed     88.76%
  19  Oreina_cacaiiae        0.00%    passed     89.38%
  20  Chrysomela_tremula     0.00%    passed     48.12%
****  TOTAL                  0.09%  0 sequences failed composition chi2 test (p-value<5%; df=3)


Create initial parsimony tree by phylogenetic likelihood library (PLL)... 0.001 seconds
NOTE: ModelFinder requires 2 MB RAM!
ModelFinder will test 286 DNA models (sample size: 553) ...
 No. Model         -LnL         df  AIC          AICc         BIC
Measuring multi-threading efficiency up to 8 CPU cores
Increase to 10 rounds for branch lengths
4590 trees examined
Threads: 1 / Time: 8.001 sec / Speedup: 1.000 / Efficiency: 100% / LogL: -4911
Threads: 2 / Time: 6.693 sec / Speedup: 1.195 / Efficiency: 60% / LogL: -4911
Threads: 3 / Time: 6.326 sec / Speedup: 1.265 / Efficiency: 42% / LogL: -4911
BEST NUMBER OF THREADS: 2

  1  JC            4062.776     37  8199.553     8205.013     8359.221
  2  JC+I          3809.450     38  7694.899     7700.666     7858.883
  3  JC+G4         3766.492     38  7608.984     7614.750     7772.967
  4  JC+I+G4       3763.459     39  7604.919     7611.001     7773.218
  5  JC+R2         3771.252     39  7620.504     7626.586     7788.803
  6  JC+R3         3763.164     41  7608.328     7615.068     7785.258
  7  JC+R4         3763.107     43  7612.215     7619.649     7797.775
 14  F81+F         3989.365     40  8058.729     8065.135     8231.344
 15  F81+F+I       3701.500     41  7484.999     7491.739     7661.929
 16  F81+F+G4      3646.779     41  7375.557     7382.297     7552.487
 17  F81+F+I+G4    3643.087     42  7370.174     7377.256     7551.419
 18  F81+F+R2      3654.003     42  7392.006     7399.088     7573.251
 19  F81+F+R3      3642.259     44  7372.518     7380.313     7562.394
 20  F81+F+R4      3642.254     46  7376.509     7385.054     7575.015
 27  K2P           3996.473     38  8068.946     8074.712     8232.929
 28  K2P+I         3741.647     39  7561.294     7567.376     7729.593
 29  K2P+G4        3695.557     39  7469.114     7475.196     7637.413
 30  K2P+I+G4      3691.035     40  7462.070     7468.477     7634.685
 31  K2P+R2        3701.282     40  7482.564     7488.970     7655.178
 32  K2P+R3        3689.815     42  7463.630     7470.713     7644.875
 33  K2P+R4        3689.774     44  7467.547     7475.342     7657.423
 40  HKY+F         3880.001     41  7842.003     7848.743     8018.933
 41  HKY+F+I       3560.106     42  7204.211     7211.294     7385.456
 42  HKY+F+G4      3489.194     42  7062.388     7069.471     7243.633
 43  HKY+F+I+G4    3480.878     43  7047.756     7055.190     7233.316
 44  HKY+F+R2      3502.832     43  7091.663     7099.097     7277.223
 45  HKY+F+R3      3478.863     45  7047.726     7055.891     7241.917
 46  HKY+F+R4      3478.837     47  7051.674     7060.609     7254.496
 53  TNe           3963.804     39  8005.609     8011.691     8173.908
 54  TNe+I         3715.582     40  7511.164     7517.571     7683.779
 55  TNe+G4        3663.096     40  7406.191     7412.597     7578.805
 56  TNe+I+G4      3654.705     41  7391.410     7398.150     7568.340
 57  TNe+R2        3675.230     41  7432.461     7439.200     7609.390
 58  TNe+R3        3649.158     43  7384.316     7391.750     7569.877
 59  TNe+R4        3649.135     45  7388.270     7396.436     7582.461
 66  TN+F          3864.168     42  7812.335     7819.417     7993.580
 67  TN+F+I        3549.491     43  7184.982     7192.416     7370.543
 68  TN+F+G4       3477.384     43  7040.768     7048.202     7226.328
 69  TN+F+I+G4     3464.930     44  7017.859     7025.654     7207.735
 70  TN+F+R2       3494.774     44  7077.548     7085.343     7267.424
 71  TN+F+R3       3460.902     46  7013.804     7022.350     7212.311
 72  TN+F+R4       3460.638     48  7017.276     7026.609     7224.413
 79  K3P           3941.180     39  7960.360     7966.442     8128.659
 80  K3P+I         3681.871     40  7443.742     7450.149     7616.357
 81  K3P+G4        3634.681     40  7349.362     7355.768     7521.976
 82  K3P+I+G4      3629.902     41  7341.804     7348.543     7518.733
 83  K3P+R2        3640.725     41  7363.450     7370.189     7540.379
 84  K3P+R3        3628.862     43  7343.724     7351.158     7529.285
 85  K3P+R4        3628.858     45  7347.715     7355.881     7541.906
 92  K3Pu+F        3861.056     42  7806.112     7813.195     7987.357
 93  K3Pu+F+I      3550.601     43  7187.202     7194.636     7372.763
 94  K3Pu+F+G4     3482.197     43  7050.394     7057.828     7235.954
 95  K3Pu+F+I+G4   3474.592     44  7037.184     7044.979     7227.059
 96  K3Pu+F+R2     3495.205     44  7078.411     7086.206     7268.287
 97  K3Pu+F+R3     3472.440     46  7036.880     7045.426     7235.387
 98  K3Pu+F+R4     3472.381     48  7040.762     7050.095     7247.899
105  TPM2+F        3850.275     42  7784.550     7791.633     7965.795
106  TPM2+F+I      3540.949     43  7167.898     7175.332     7353.459
107  TPM2+F+G4     3479.103     43  7044.207     7051.641     7229.767
108  TPM2+F+I+G4   3472.600     44  7033.200     7040.996     7223.076
109  TPM2+F+R2     3489.731     44  7067.462     7075.258     7257.338
110  TPM2+F+R3     3471.407     46  7034.815     7043.360     7233.321
111  TPM2+F+R4     3471.330     48  7038.660     7047.994     7245.797
118  TPM2u+F       3850.273     42  7784.546     7791.629     7965.791
119  TPM2u+F+I     3540.950     43  7167.900     7175.334     7353.460
120  TPM2u+F+G4    3479.104     43  7044.209     7051.643     7229.769
121  TPM2u+F+I+G4  3472.601     44  7033.201     7040.997     7223.077
122  TPM2u+F+R2    3489.729     44  7067.458     7075.254     7257.334
123  TPM2u+F+R3    3471.366     46  7034.732     7043.278     7233.239
124  TPM2u+F+R4    3471.346     48  7038.691     7048.024     7245.828
131  TPM3+F        3874.057     42  7832.114     7839.196     8013.359
132  TPM3+F+I      3559.582     43  7205.164     7212.598     7390.725
133  TPM3+F+G4     3488.871     43  7063.742     7071.176     7249.303
134  TPM3+F+I+G4   3480.593     44  7049.187     7056.982     7239.062
135  TPM3+F+R2     3502.684     44  7093.368     7101.163     7283.243
136  TPM3+F+R3     3478.477     46  7048.953     7057.499     7247.460
137  TPM3+F+R4     3478.411     48  7052.823     7062.156     7259.960
144  TPM3u+F       3874.057     42  7832.113     7839.195     8013.358
145  TPM3u+F+I     3559.581     43  7205.161     7212.595     7390.721
146  TPM3u+F+G4    3488.870     43  7063.740     7071.174     7249.300
147  TPM3u+F+I+G4  3480.575     44  7049.149     7056.945     7239.025
148  TPM3u+F+R2    3502.684     44  7093.368     7101.163     7283.243
149  TPM3u+F+R3    3478.434     46  7048.869     7057.414     7247.375
150  TPM3u+F+R4    3478.381     48  7052.763     7062.096     7259.900
157  TIMe          3907.288     40  7894.576     7900.982     8067.190
158  TIMe+I        3654.189     41  7390.378     7397.118     7567.308
159  TIMe+G4       3601.660     41  7285.319     7292.059     7462.249
160  TIMe+I+G4     3593.591     42  7271.183     7278.265     7452.428
161  TIMe+R2       3613.704     42  7311.408     7318.490     7492.653
162  TIMe+R3       3589.487     44  7266.973     7274.769     7456.849
163  TIMe+R4       3589.453     46  7270.907     7279.452     7469.413
170  TIM+F         3844.902     43  7775.804     7783.238     7961.365
171  TIM+F+I       3539.259     44  7166.518     7174.313     7356.394
172  TIM+F+G4      3468.917     44  7025.834     7033.629     7215.710
173  TIM+F+I+G4    3457.529     45  7005.058     7013.224     7199.249
174  TIM+F+R2      3484.715     45  7059.431     7067.596     7253.622
175  TIM+F+R3      3453.037     47  7000.075     7009.009     7202.897
176  TIM+F+R4      3452.996     49  7003.993     7013.734     7215.445
183  TIM2e         3888.299     40  7856.599     7863.005     8029.213
184  TIM2e+I       3644.593     41  7371.187     7377.926     7548.116
185  TIM2e+G4      3595.369     41  7272.738     7279.478     7449.668
186  TIM2e+I+G4    3590.392     42  7264.783     7271.865     7446.028
187  TIM2e+R2      3603.494     42  7290.989     7298.071     7472.234
188  TIM2e+R3      3588.104     44  7264.208     7272.003     7454.084
189  TIM2e+R4      3588.102     46  7268.203     7276.749     7466.710
196  TIM2+F        3835.055     43  7756.110     7763.544     7941.670
197  TIM2+F+I      3530.882     44  7149.765     7157.560     7339.640
198  TIM2+F+G4     3465.624     44  7019.248     7027.043     7209.123
199  TIM2+F+I+G4   3454.720     45  6999.439     7007.605     7193.630
200  TIM2+F+R2     3479.012     45  7048.024     7056.190     7242.215
201  TIM2+F+R3     3450.711     47  6995.422     7004.357     7198.244
202  TIM2+F+R4     3450.673     49  6999.346     7009.087     7210.798
209  TIM3e         3937.908     40  7955.816     7962.222     8128.430
210  TIM3e+I       3703.598     41  7489.195     7495.935     7666.125
211  TIM3e+G4      3646.460     41  7374.920     7381.660     7551.850
212  TIM3e+I+G4    3637.794     42  7359.589     7366.671     7540.834
213  TIM3e+R2      3660.767     42  7405.535     7412.617     7586.780
214  TIM3e+R3      3631.066     44  7350.133     7357.928     7540.009
215  TIM3e+R4      3631.059     46  7354.118     7362.663     7552.624
222  TIM3+F        3858.091     43  7802.183     7809.617     7987.743
223  TIM3+F+I      3548.899     44  7185.798     7193.593     7375.673
224  TIM3+F+G4     3477.223     44  7042.445     7050.241     7232.321
225  TIM3+F+I+G4   3464.860     45  7019.721     7027.886     7213.912
226  TIM3+F+R2     3494.497     45  7078.994     7087.160     7273.185
227  TIM3+F+R3     3460.825     47  7015.651     7024.586     7218.473
228  TIM3+F+R4     3459.985     49  7017.970     7027.712     7229.423
235  TVMe          3886.996     41  7855.992     7862.731     8032.921
236  TVMe+I        3647.165     42  7378.330     7385.412     7559.575
237  TVMe+G4       3597.921     42  7279.841     7286.924     7461.086
238  TVMe+I+G4     3594.938     43  7275.876     7283.310     7461.437
239  TVMe+R2       3602.644     43  7291.287     7298.722     7476.848
240  TVMe+R3       3594.156     45  7278.311     7286.477     7472.502
241  TVMe+R4       3594.091     47  7282.182     7291.117     7485.004
248  TVM+F         3843.560     44  7775.120     7782.915     7964.996
249  TVM+F+I       3539.765     45  7169.530     7177.695     7363.721
250  TVM+F+G4      3476.505     45  7043.010     7051.176     7237.201
251  TVM+F+I+G4    3469.314     46  7030.628     7039.173     7229.134
252  TVM+F+R2      3487.022     46  7066.044     7074.589     7264.550
253  TVM+F+R3      3468.533     48  7033.066     7042.399     7240.203
254  TVM+F+R4      3467.969     50  7035.938     7046.097     7251.706
261  SYM           3854.701     42  7793.401     7800.484     7974.646
262  SYM+I         3620.972     43  7327.944     7335.378     7513.504
263  SYM+G4        3567.884     43  7221.768     7229.202     7407.329
264  SYM+I+G4      3561.330     44  7210.659     7218.454     7400.535
265  SYM+R2        3578.160     44  7244.320     7252.115     7434.195
266  SYM+R3        3557.646     46  7207.292     7215.837     7405.798
267  SYM+R4        3557.594     48  7211.188     7220.521     7418.325
274  GTR+F         3828.175     45  7746.350     7754.516     7940.541
275  GTR+F+I       3529.503     46  7151.005     7159.551     7349.512
276  GTR+F+G4      3462.821     46  7017.642     7026.187     7216.148
277  GTR+F+I+G4    3451.980     47  6997.959     7006.894     7200.781
278  GTR+F+R2      3476.072     47  7046.144     7055.078     7248.966
279  GTR+F+R3      3448.235     49  6994.470     7004.211     7205.922
280  GTR+F+R4      3448.177     51  6998.353     7008.940     7218.436
Akaike Information Criterion:           GTR+F+R3
Corrected Akaike Information Criterion: GTR+F+R3
Bayesian Information Criterion:         TIM2+F+I+G4
Best-fit model: TIM2+F+I+G4 chosen according to BIC

All model information printed to beetles_COII_data.fasta.model.gz
CPU time for ModelFinder: 45.796 seconds (0h:0m:45s)
Wall-clock time for ModelFinder: 23.373 seconds (0h:0m:23s)
Generating 1000 samples for ultrafast bootstrap (seed: 219955)...

NOTE: 1 MB RAM (0 GB) is required!
Measuring multi-threading efficiency up to 8 CPU cores
Increase to 10 rounds for branch lengths
1308 trees examined
Threads: 1 / Time: 8.000 sec / Speedup: 1.000 / Efficiency: 100% / LogL: -4083
Threads: 2 / Time: 4.986 sec / Speedup: 1.604 / Efficiency: 80% / LogL: -4083
Threads: 3 / Time: 5.183 sec / Speedup: 1.544 / Efficiency: 51% / LogL: -4083
Threads: 4 / Time: 6.347 sec / Speedup: 1.260 / Efficiency: 32% / LogL: -4083
BEST NUMBER OF THREADS: 2

Estimate model parameters (epsilon = 0.100)
Thoroughly optimizing +I+G parameters from 10 start values...
Init pinv, alpha: 0.000, 1.000 / Estimate: 0.000, 0.232 / LogL: -3465.600
Init pinv, alpha: 0.065, 1.000 / Estimate: 0.304, 0.361 / LogL: -3454.957
Init pinv, alpha: 0.131, 1.000 / Estimate: 0.303, 0.360 / LogL: -3454.970
Init pinv, alpha: 0.196, 1.000 / Estimate: 0.303, 0.360 / LogL: -3454.959
Init pinv, alpha: 0.261, 1.000 / Estimate: 0.308, 0.368 / LogL: -3454.905
Init pinv, alpha: 0.327, 1.000 / Estimate: 0.337, 0.402 / LogL: -3454.675
Init pinv, alpha: 0.392, 1.000 / Estimate: 0.379, 0.456 / LogL: -3454.661
Init pinv, alpha: 0.457, 1.000 / Estimate: 0.396, 0.478 / LogL: -3454.774
Init pinv, alpha: 0.522, 1.000 / Estimate: 0.402, 0.486 / LogL: -3454.836
Init pinv, alpha: 0.588, 1.000 / Estimate: 0.402, 0.485 / LogL: -3454.832
Optimal pinv,alpha: 0.379, 0.456 / LogL: -3454.661

Parameters optimization took 0.346 sec
Computing ML distances based on estimated model parameters... 0.003 sec
Computing BIONJ tree...
0.001 seconds
Log-likelihood of BIONJ tree: -3452.176
--------------------------------------------------------------------
|             INITIALIZING CANDIDATE TREE SET                      |
--------------------------------------------------------------------
Generating 98 parsimony trees... 0.059 second
Computing log-likelihood of 98 initial trees ... 0.112 seconds
Current best score: -3452.176

Do NNI search on 20 best initial trees
Estimate model parameters (epsilon = 0.100)
BETTER TREE FOUND at iteration 1: -3450.744
Estimate model parameters (epsilon = 0.100)
BETTER TREE FOUND at iteration 4: -3449.528
Iteration 10 / LogL: -3451.173 / Time: 0h:0m:25s
Iteration 20 / LogL: -3451.378 / Time: 0h:0m:25s
Finish initializing candidate tree set (6)
Current best tree score: -3449.528 / CPU time: 0.377
Number of iterations: 20
--------------------------------------------------------------------
|               OPTIMIZING CANDIDATE TREE SET                      |
--------------------------------------------------------------------
Estimate model parameters (epsilon = 0.100)
BETTER TREE FOUND at iteration 24: -3448.976
Iteration 30 / LogL: -3449.040 / Time: 0h:0m:25s (0h:1m:22s left)
Iteration 40 / LogL: -3449.571 / Time: 0h:0m:25s (0h:0m:55s left)
Iteration 50 / LogL: -3450.760 / Time: 0h:0m:25s (0h:0m:38s left)
Log-likelihood cutoff on original alignment: -3473.945
Iteration 60 / LogL: -3450.843 / Time: 0h:0m:25s (0h:0m:28s left)
Iteration 70 / LogL: -3450.077 / Time: 0h:0m:26s (0h:0m:20s left)
Iteration 80 / LogL: -3450.729 / Time: 0h:0m:26s (0h:0m:14s left)
Iteration 90 / LogL: -3450.186 / Time: 0h:0m:26s (0h:0m:10s left)
Iteration 100 / LogL: -3449.628 / Time: 0h:0m:26s (0h:0m:6s left)
Log-likelihood cutoff on original alignment: -3473.008
NOTE: Bootstrap correlation coefficient of split occurrence frequencies: 0.998
Iteration 110 / LogL: -3449.677 / Time: 0h:0m:26s (0h:0m:22s left)
Iteration 120 / LogL: -3450.966 / Time: 0h:0m:26s (0h:0m:18s left)
TREE SEARCH COMPLETED AFTER 125 ITERATIONS / Time: 0h:0m:27s

--------------------------------------------------------------------
|                    FINALIZING TREE SEARCH                        |
--------------------------------------------------------------------
Performs final model parameters optimization
Estimate model parameters (epsilon = 0.010)
1. Initial log-likelihood: -3448.976
Optimal log-likelihood: -3448.971
Rate parameters:  A-C: 5.05178  A-G: 13.38183  A-T: 5.05178  C-G: 1.00000  C-T: 45.47700  G-T: 1.00000
Base frequencies:  A: 0.351  C: 0.157  G: 0.111  T: 0.381
Proportion of invariable sites: 0.369
Gamma shape alpha: 0.427
Parameters optimization took 1 rounds (0.003 sec)
BEST SCORE FOUND : -3448.971
Creating bootstrap support values...
Split supports printed to NEXUS file beetles_COII_data.fasta.splits.nex
Total tree length: 3.217

Total number of iterations: 125
CPU time used for tree search: 4.135 sec (0h:0m:4s)
Wall-clock time used for tree search: 2.161 sec (0h:0m:2s)
Total CPU time used: 61.760 sec (0h:1m:1s)
Total wall-clock time used: 27.088 sec (0h:0m:27s)

Computing bootstrap consensus tree...
Reading input file beetles_COII_data.fasta.splits.nex...
20 taxa and 230 splits.
Consensus tree written to beetles_COII_data.fasta.contree
Reading input trees file beetles_COII_data.fasta.contree
Log-likelihood of consensus tree: -3448.971

Analysis results written to: 
  IQ-TREE report:                beetles_COII_data.fasta.iqtree
  Maximum-likelihood tree:       beetles_COII_data.fasta.treefile
  Likelihood distances:          beetles_COII_data.fasta.mldist

Ultrafast bootstrap approximation results written to:
  Split support values:          beetles_COII_data.fasta.splits.nex
  Consensus tree:                beetles_COII_data.fasta.contree
  Screen log file:               beetles_COII_data.fasta.log

Date and Time: Tue May  2 13:55:11 2023
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git add .
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git commit -m "updated files and folders"
[master 2b8b5e6] updated files and folders
 Committer: Aidyn Kehrli <aidynkehrli@Aidyns-MacBook-Pro.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 12 files changed, 982 insertions(+)
 create mode 100644 beetles_COII_data.fasta.bionj
 create mode 100644 beetles_COII_data.fasta.ckp.gz
 create mode 100644 beetles_COII_data.fasta.contree
 create mode 100644 beetles_COII_data.fasta.iqtree
 create mode 100644 beetles_COII_data.fasta.log
 create mode 100644 beetles_COII_data.fasta.mldist
 create mode 100644 beetles_COII_data.fasta.model.gz
 create mode 100644 beetles_COII_data.fasta.splits.nex
 create mode 100644 beetles_COII_data.fasta.treefile
 create mode 100755 iqtree
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git push
Enumerating objects: 19, done.
Counting objects: 100% (19/19), done.
Delta compression using up to 8 threads
Compressing objects: 100% (15/15), done.
Writing objects: 100% (15/15), 2.74 MiB | 3.52 MiB/s, done.
Total 15 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), completed with 4 local objects.
To https://github.com/aidynkehrli/Botany-563.git
   7d3491c..2b8b5e6  master -> master
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % pwd
/Users/aidynkehrli/Desktop/Botany-563
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % cd iqtree 
cd: not a directory: iqtree
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % //
zsh: permission denied: //
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % ls
3-30-homework-test			beetles_16s_data.fasta
3-30-homework-test.bionj		beetles_COII_data.fasta
3-30-homework-test.ckp.gz		beetles_COII_data.fasta.bionj
3-30-homework-test.iqtree		beetles_COII_data.fasta.ckp.gz
3-30-homework-test.log			beetles_COII_data.fasta.contree
3-30-homework-test.mldist		beetles_COII_data.fasta.iqtree
3-30-homework-test.model		beetles_COII_data.fasta.log
3-30-homework-test.model.gz		beetles_COII_data.fasta.mldist
3-30-homework-test.treefile		beetles_COII_data.fasta.model.gz
30 Homework Test			beetles_COII_data.fasta.splits.nex
Analysis				beetles_COII_data.fasta.treefile
Data					beetles_COII_data2.fasta
Figures					data_clean
R Console.txt				data_raw
R_tree_12s_data.pdf			iqtree
R_tree_16s_data.pdf			iqtree-1.6.12-MacOSX
R_tree_COII_data.pdf			notebook-log.md
Terminal Saved Output.txt		readme.md
beetles_12s_data.fasta
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % cd iqtree-1.6.12-MacOSX 
(base) aidynkehrli@Aidyns-MacBook-Pro iqtree-1.6.12-MacOSX % cd bin 
(base) aidynkehrli@Aidyns-MacBook-Pro bin % iqtree -s beetles_12s_data.fasta -bb 1000 -nt AUTO
zsh: command not found: iqtree
(base) aidynkehrli@Aidyns-MacBook-Pro bin % pwd
/Users/aidynkehrli/Desktop/Botany-563/iqtree-1.6.12-MacOSX/bin
(base) aidynkehrli@Aidyns-MacBook-Pro bin % 
(base) aidynkehrli@Aidyns-MacBook-Pro bin % iqtree -s beetles_12s_data.fasta -bb 1000 -nt AUTO
zsh: command not found: iqtree
(base) aidynkehrli@Aidyns-MacBook-Pro bin % cd iqtree-1.6.12-MacOSX                              
cd: no such file or directory: iqtree-1.6.12-MacOSX
(base) aidynkehrli@Aidyns-MacBook-Pro bin % pwd                                               
/Users/aidynkehrli/Desktop/Botany-563/iqtree-1.6.12-MacOSX/bin
(base) aidynkehrli@Aidyns-MacBook-Pro bin % ls                                                
iqtree
(base) aidynkehrli@Aidyns-MacBook-Pro bin % cd iqtree                                         
cd: not a directory: iqtree
(base) aidynkehrli@Aidyns-MacBook-Pro bin % //                                                
zsh: permission denied: //
(base) aidynkehrli@Aidyns-MacBook-Pro bin % ./iqtree -s beetles_12s_data.fasta iqtree -s beetles_12s_data.fasta -bb 1000 -nt AUTO
IQ-TREE multicore version 1.6.12 for Mac OS X 64-bit built Aug 15 2019
Developed by Bui Quang Minh, Nguyen Lam Tung, Olga Chernomor,
Heiko Schmidt, Dominik Schrempf, Michael Woodhams.

Host:    Aidyns-MacBook-Pro.local (SSE4.2, 8 GB RAM)
Command: ./iqtree -s beetles_12s_data.fasta iqtree -s beetles_12s_data.fasta -bb 1000 -nt AUTO
Seed:    455387 (Using SPRNG - Scalable Parallel Random Number Generator)
Time:    Wed May  3 12:20:19 2023
Kernel:  SSE2 - auto-detect threads (8 CPU cores detected)

Reading alignment file beetles_12s_data.fasta ... ERROR: File not found beetles_12s_data.fasta
(base) aidynkehrli@Aidyns-MacBook-Pro bin % iqtree -s beetles_12s_data.fasta -bb 1000 -nt AUTO
zsh: command not found: iqtree
(base) aidynkehrli@Aidyns-MacBook-Pro bin % ./iqtree -s beetles_12s_data.fasta -bb 1000 -nt AUTO
IQ-TREE multicore version 1.6.12 for Mac OS X 64-bit built Aug 15 2019
Developed by Bui Quang Minh, Nguyen Lam Tung, Olga Chernomor,
Heiko Schmidt, Dominik Schrempf, Michael Woodhams.

Host:    Aidyns-MacBook-Pro.local (SSE4.2, 8 GB RAM)
Command: ./iqtree -s beetles_12s_data.fasta -bb 1000 -nt AUTO
Seed:    319039 (Using SPRNG - Scalable Parallel Random Number Generator)
Time:    Wed May  3 12:20:50 2023
Kernel:  SSE2 - auto-detect threads (8 CPU cores detected)

Reading alignment file beetles_12s_data.fasta ... ERROR: File not found beetles_12s_data.fasta
(base) aidynkehrli@Aidyns-MacBook-Pro bin % iqtree -s beetles_12s_data -bb 1000 -nt AUTO       
zsh: command not found: iqtree
(base) aidynkehrli@Aidyns-MacBook-Pro bin % ./iqtree -s beetles_12s_data -bb 1000 -nt AUTO       
IQ-TREE multicore version 1.6.12 for Mac OS X 64-bit built Aug 15 2019
Developed by Bui Quang Minh, Nguyen Lam Tung, Olga Chernomor,
Heiko Schmidt, Dominik Schrempf, Michael Woodhams.

Host:    Aidyns-MacBook-Pro.local (SSE4.2, 8 GB RAM)
Command: ./iqtree -s beetles_12s_data -bb 1000 -nt AUTO
Seed:    925859 (Using SPRNG - Scalable Parallel Random Number Generator)
Time:    Wed May  3 12:22:50 2023
Kernel:  SSE2 - auto-detect threads (8 CPU cores detected)

Reading alignment file beetles_12s_data ... ERROR: File not found beetles_12s_data
(base) aidynkehrli@Aidyns-MacBook-Pro bin % ls
beetles_12s_data.fasta.log	beetles_12s_data.log		iqtree
(base) aidynkehrli@Aidyns-MacBook-Pro bin % iqtree -s beetles_12s_data.fasta.log -bb 1000 -nt AUTO
zsh: command not found: iqtree
(base) aidynkehrli@Aidyns-MacBook-Pro bin % ./iqtree -s beetles_12s_data.fasta.log -bb 1000 -nt AUTO 
IQ-TREE multicore version 1.6.12 for Mac OS X 64-bit built Aug 15 2019
Developed by Bui Quang Minh, Nguyen Lam Tung, Olga Chernomor,
Heiko Schmidt, Dominik Schrempf, Michael Woodhams.

Host:    Aidyns-MacBook-Pro.local (SSE4.2, 8 GB RAM)
Command: ./iqtree -s beetles_12s_data.fasta.log -bb 1000 -nt AUTO
Seed:    643747 (Using SPRNG - Scalable Parallel Random Number Generator)
Time:    Wed May  3 12:23:52 2023
Kernel:  SSE2 - auto-detect threads (8 CPU cores detected)

Reading alignment file beetles_12s_data.fasta.log ... ERROR: Unknown sequence format, please use PHYLIP, FASTA, CLUSTAL, MSF, or NEXUS format
(base) aidynkehrli@Aidyns-MacBook-Pro bin % ls
beetles_12s_data.fasta.log	beetles_12s_data.log
beetles_12s_data.fasta.log.log	iqtree
(base) aidynkehrli@Aidyns-MacBook-Pro bin % ./iqtree -s beetles_12s_data.log -bb 1000 -nt AUTO
IQ-TREE multicore version 1.6.12 for Mac OS X 64-bit built Aug 15 2019
Developed by Bui Quang Minh, Nguyen Lam Tung, Olga Chernomor,
Heiko Schmidt, Dominik Schrempf, Michael Woodhams.

Host:    Aidyns-MacBook-Pro.local (SSE4.2, 8 GB RAM)
Command: ./iqtree -s beetles_12s_data.log -bb 1000 -nt AUTO
Seed:    640817 (Using SPRNG - Scalable Parallel Random Number Generator)
Time:    Wed May  3 12:26:10 2023
Kernel:  SSE2 - auto-detect threads (8 CPU cores detected)

Reading alignment file beetles_12s_data.log ... ERROR: Unknown sequence format, please use PHYLIP, FASTA, CLUSTAL, MSF, or NEXUS format
(base) aidynkehrli@Aidyns-MacBook-Pro bin % ./iqtree -s beetles_12s_data.fasta -bb 1000 -nt AUTO
IQ-TREE multicore version 1.6.12 for Mac OS X 64-bit built Aug 15 2019
Developed by Bui Quang Minh, Nguyen Lam Tung, Olga Chernomor,
Heiko Schmidt, Dominik Schrempf, Michael Woodhams.

Host:    Aidyns-MacBook-Pro.local (SSE4.2, 8 GB RAM)
Command: ./iqtree -s beetles_12s_data.fasta -bb 1000 -nt AUTO
Seed:    109030 (Using SPRNG - Scalable Parallel Random Number Generator)
Time:    Wed May  3 12:26:42 2023
Kernel:  SSE2 - auto-detect threads (8 CPU cores detected)

Reading alignment file beetles_12s_data.fasta ... ERROR: File not found beetles_12s_data.fasta
(base) aidynkehrli@Aidyns-MacBook-Pro bin % .//
zsh: permission denied: .//
(base) aidynkehrli@Aidyns-MacBook-Pro bin % cd ..                                                
(base) aidynkehrli@Aidyns-MacBook-Pro iqtree-1.6.12-MacOSX % ./iqtree -s beetles_12s_data.fasta -bb 1000 -nt AUTO
zsh: no such file or directory: ./iqtree
(base) aidynkehrli@Aidyns-MacBook-Pro iqtree-1.6.12-MacOSX % cd iqtree-1.6.12-MacOSX
cd: no such file or directory: iqtree-1.6.12-MacOSX
(base) aidynkehrli@Aidyns-MacBook-Pro iqtree-1.6.12-MacOSX % cd bin
(base) aidynkehrli@Aidyns-MacBook-Pro bin % ./iqtree -s beetles_12s_data.fasta -bb 1000 -nt AUTO
IQ-TREE multicore version 1.6.12 for Mac OS X 64-bit built Aug 15 2019
Developed by Bui Quang Minh, Nguyen Lam Tung, Olga Chernomor,
Heiko Schmidt, Dominik Schrempf, Michael Woodhams.

Host:    Aidyns-MacBook-Pro.local (SSE4.2, 8 GB RAM)
Command: ./iqtree -s beetles_12s_data.fasta -bb 1000 -nt AUTO
Seed:    500793 (Using SPRNG - Scalable Parallel Random Number Generator)
Time:    Wed May  3 12:28:53 2023
Kernel:  SSE2 - auto-detect threads (8 CPU cores detected)

Reading alignment file beetles_12s_data.fasta ... ERROR: File not found beetles_12s_data.fasta
(base) aidynkehrli@Aidyns-MacBook-Pro bin % ls
beetles_12s_data.fasta.log	beetles_12s_data.log		iqtree
beetles_12s_data.fasta.log.log	beetles_12s_data.log.log
(base) aidynkehrli@Aidyns-MacBook-Pro bin % pwd
/Users/aidynkehrli/Desktop/Botany-563/iqtree-1.6.12-MacOSX/bin
(base) aidynkehrli@Aidyns-MacBook-Pro bin % cd..
zsh: command not found: cd..
(base) aidynkehrli@Aidyns-MacBook-Pro bin % cd..
zsh: command not found: cd..
(base) aidynkehrli@Aidyns-MacBook-Pro bin % cd..
zsh: command not found: cd..
(base) aidynkehrli@Aidyns-MacBook-Pro bin % iqtree-1.6.12-MacOSX % cd ..
zsh: command not found: iqtree-1.6.12-MacOSX
(base) aidynkehrli@Aidyns-MacBook-Pro bin % cd..
zsh: command not found: cd..
(base) aidynkehrli@Aidyns-MacBook-Pro bin % cd..
zsh: command not found: cd..
(base) aidynkehrli@Aidyns-MacBook-Pro bin % cd
(base) aidynkehrli@Aidyns-MacBook-Pro ~ % cd Botany-563 
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % ls
Analysis	Figures		data_clean	notebook-log.md
Data		README.md	data_raw
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % ls
Analysis	Figures		data_clean	notebook-log.md
Data		README.md	data_raw
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % pwd
/Users/aidynkehrli/Botany-563
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % cd..
zsh: command not found: cd..
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % ls
Analysis	Figures		data_clean	notebook-log.md
Data		README.md	data_raw
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % /iqtree -s beetles_COII_data.fasta -bb 1000 -nt AUTO

zsh: no such file or directory: /iqtree
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % pwd
/Users/aidynkehrli/Botany-563
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % cd Desktop
cd: no such file or directory: Desktop
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % cd
(base) aidynkehrli@Aidyns-MacBook-Pro ~ % cd Desktop 
(base) aidynkehrli@Aidyns-MacBook-Pro Desktop % cd Botany-563 
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % ls
3-30-homework-test			beetles_16s_data.fasta
3-30-homework-test.bionj		beetles_COII_data.fasta
3-30-homework-test.ckp.gz		beetles_COII_data.fasta.bionj
3-30-homework-test.iqtree		beetles_COII_data.fasta.ckp.gz
3-30-homework-test.log			beetles_COII_data.fasta.contree
3-30-homework-test.mldist		beetles_COII_data.fasta.iqtree
3-30-homework-test.model		beetles_COII_data.fasta.log
3-30-homework-test.model.gz		beetles_COII_data.fasta.mldist
3-30-homework-test.treefile		beetles_COII_data.fasta.model.gz
30 Homework Test			beetles_COII_data.fasta.splits.nex
Analysis				beetles_COII_data.fasta.treefile
Data					beetles_COII_data2.fasta
Figures					data_clean
R Console.txt				data_raw
R_tree_12s_data.pdf			iqtree
R_tree_16s_data.pdf			iqtree-1.6.12-MacOSX
R_tree_COII_data.pdf			notebook-log.md
Terminal Saved Output.txt		readme.md
beetles_12s_data.fasta
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % /iqtree -s beetles_12s_data.fasta -bb 1000 -nt AUTO
zsh: no such file or directory: /iqtree
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % ./iqtree -s beetles_12s_data.fasta -bb 1000 -nt AUTO
IQ-TREE multicore version 1.6.12 for Mac OS X 64-bit built Aug 15 2019
Developed by Bui Quang Minh, Nguyen Lam Tung, Olga Chernomor,
Heiko Schmidt, Dominik Schrempf, Michael Woodhams.

Host:    Aidyns-MacBook-Pro.local (SSE4.2, 8 GB RAM)
Command: ./iqtree -s beetles_12s_data.fasta -bb 1000 -nt AUTO
Seed:    463336 (Using SPRNG - Scalable Parallel Random Number Generator)
Time:    Wed May  3 12:38:13 2023
Kernel:  SSE2 - auto-detect threads (8 CPU cores detected)

Reading alignment file beetles_12s_data.fasta ... Fasta format detected
Alignment most likely contains DNA/RNA sequences
WARNING: 1 sites contain only gaps or ambiguous characters.
ERROR: Sequence G_viminalis_1 has invalid character 0 at site 354
ERROR: Sequence G_olivacea_1 has invalid character 0 at site 354
ERROR: Sequence G_rufipes has invalid character 0 at site 354
ERROR: Sequence G_linnaeana has invalid character 0 at site 354
ERROR: Sequence G_variabilis_1 has invalid character 0 at site 354
ERROR: Sequence G_fornicata has invalid character 0 at site 354
ERROR: Sequence G_occidentalis has invalid character 0 at site 354
ERROR: Sequence G_interposita_1 has invalid character 0 at site 354
ERROR: Sequence G_interposita_2 has invalid character 0 at site 354
ERROR: Sequence G_intermedia has invalid character 0 at site 354
ERROR: Sequence G_quinquepunctata_2 has invalid character 0 at site 354
ERROR: Sequence G_holdausi has invalid character 0 at site 354
ERROR: Sequence G_pallida_2 has invalid character 0 at site 354
ERROR: Sequence G_pallida_3 has invalid character 0 at site 354
ERROR: Sequence G_tredecimmaculata has invalid character 0 at site 354
ERROR: Sequence G_nigropiagiata has invalid character 0 at site 354
ERROR: Sequence G_kamikawai has invalid character 0 at site 354
ERROR: Sequence G_rubripennis has invalid character 0 at site 354
ERROR: Sequence Oreina_cacaiiae has invalid character 0 at site 354
ERROR: Sequence Chrysomela_tremula has invalid character 1 at site 354
ERROR: Sequence G_viminalis_1 has invalid character 1 at site 355
ERROR: Sequence G_olivacea_1 has invalid character 1 at site 355
ERROR: Sequence G_rufipes has invalid character 1 at site 355
ERROR: Sequence G_linnaeana has invalid character 1 at site 355
ERROR: Sequence G_variabilis_1 has invalid character 1 at site 355
ERROR: Sequence G_fornicata has invalid character 1 at site 355
ERROR: Sequence G_occidentalis has invalid character 1 at site 355
ERROR: Sequence G_interposita_1 has invalid character 1 at site 355
ERROR: Sequence G_interposita_2 has invalid character 1 at site 355
ERROR: Sequence G_intermedia has invalid character 1 at site 355
ERROR: Sequence G_quinquepunctata_2 has invalid character 1 at site 355
ERROR: Sequence G_holdausi has invalid character 1 at site 355
ERROR: Sequence G_pallida_2 has invalid character 1 at site 355
ERROR: Sequence G_pallida_3 has invalid character 1 at site 355
ERROR: Sequence G_tredecimmaculata has invalid character 1 at site 355
ERROR: Sequence G_nigropiagiata has invalid character 0 at site 355
ERROR: Sequence G_kamikawai has invalid character 1 at site 355
ERROR: Sequence G_rubripennis has invalid character 1 at site 355
ERROR: Sequence Oreina_cacaiiae has invalid character 1 at site 355
ERROR: Sequence Chrysomela_tremula has invalid character 1 at site 355
ERROR: Sequence G_viminalis_1 has invalid character 1 at site 356
ERROR: Sequence G_olivacea_1 has invalid character 1 at site 356
ERROR: Sequence G_rufipes has invalid character 1 at site 356
ERROR: Sequence G_linnaeana has invalid character 1 at site 356
ERROR: Sequence G_variabilis_1 has invalid character 1 at site 356
ERROR: Sequence G_fornicata has invalid character 1 at site 356
ERROR: Sequence G_occidentalis has invalid character 1 at site 356
ERROR: Sequence G_interposita_1 has invalid character 1 at site 356
ERROR: Sequence G_interposita_2 has invalid character 1 at site 356
ERROR: Sequence G_intermedia has invalid character 1 at site 356
ERROR: Sequence G_quinquepunctata_2 has invalid character 1 at site 356
ERROR: Sequence G_holdausi has invalid character 1 at site 356
ERROR: Sequence G_pallida_2 has invalid character 1 at site 356
ERROR: Sequence G_pallida_3 has invalid character 1 at site 356
ERROR: Sequence G_tredecimmaculata has invalid character 1 at site 356
ERROR: Sequence G_nigropiagiata has invalid character 1 at site 356
ERROR: Sequence G_kamikawai has invalid character 1 at site 356
ERROR: Sequence G_rubripennis has invalid character 1 at site 356
ERROR: Sequence Oreina_cacaiiae has invalid character 0 at site 356
ERROR: Sequence Chrysomela_tremula has invalid character 1 at site 356
ERROR: Sequence G_viminalis_1 has invalid character 0 at site 357
ERROR: Sequence G_olivacea_1 has invalid character 1 at site 357
ERROR: Sequence G_rufipes has invalid character 0 at site 357
ERROR: Sequence G_linnaeana has invalid character 0 at site 357
ERROR: Sequence G_variabilis_1 has invalid character 0 at site 357
ERROR: Sequence G_fornicata has invalid character 0 at site 357
ERROR: Sequence G_occidentalis has invalid character 0 at site 357
ERROR: Sequence G_interposita_1 has invalid character 0 at site 357
ERROR: Sequence G_interposita_2 has invalid character 0 at site 357
ERROR: Sequence G_intermedia has invalid character 0 at site 357
ERROR: Sequence G_quinquepunctata_2 has invalid character 0 at site 357
ERROR: Sequence G_holdausi has invalid character 0 at site 357
ERROR: Sequence G_pallida_2 has invalid character 0 at site 357
ERROR: Sequence G_pallida_3 has invalid character 0 at site 357
ERROR: Sequence G_tredecimmaculata has invalid character 0 at site 357
ERROR: Sequence G_nigropiagiata has invalid character 0 at site 357
ERROR: Sequence G_kamikawai has invalid character 0 at site 357
ERROR: Sequence G_rubripennis has invalid character 0 at site 357
ERROR: Sequence Oreina_cacaiiae has invalid character 0 at site 357
ERROR: Sequence Chrysomela_tremula has invalid character 0 at site 357
ERROR: Sequence G_viminalis_1 has invalid character 0 at site 358
ERROR: Sequence G_olivacea_1 has invalid character 0 at site 358
ERROR: Sequence G_rufipes has invalid character 0 at site 358
ERROR: Sequence G_linnaeana has invalid character 1 at site 358
ERROR: Sequence G_variabilis_1 has invalid character 0 at site 358
ERROR: Sequence G_fornicata has invalid character 0 at site 358
ERROR: Sequence G_occidentalis has invalid character 0 at site 358
ERROR: Sequence G_interposita_1 has invalid character 0 at site 358
ERROR: Sequence G_interposita_2 has invalid character 0 at site 358
ERROR: Sequence G_intermedia has invalid character 0 at site 358
ERROR: Sequence G_quinquepunctata_2 has invalid character 0 at site 358
ERROR: Sequence G_holdausi has invalid character 0 at site 358
ERROR: Sequence G_pallida_2 has invalid character 0 at site 358
ERROR: Sequence G_pallida_3 has invalid character 0 at site 358
ERROR: Sequence G_tredecimmaculata has invalid character 0 at site 358
ERROR: Sequence G_nigropiagiata has invalid character 0 at site 358
ERROR: Sequence G_kamikawai has invalid character 0 at site 358
ERROR: Sequence G_rubripennis has invalid character 0 at site 358
ERROR: Sequence Oreina_cacaiiae has invalid character 0 at site 358
ERROR: Sequence Chrysomela_tremula has invalid character 0 at site 358
ERROR: ...many more...
ERROR: 
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % ./iqtree -s beetles_12s_data.fasta -bb 1000 -nt AUTO

IQ-TREE multicore version 1.6.12 for Mac OS X 64-bit built Aug 15 2019
Developed by Bui Quang Minh, Nguyen Lam Tung, Olga Chernomor,
Heiko Schmidt, Dominik Schrempf, Michael Woodhams.

Host:    Aidyns-MacBook-Pro.local (SSE4.2, 8 GB RAM)
Command: ./iqtree -s beetles_12s_data.fasta -bb 1000 -nt AUTO
Seed:    180988 (Using SPRNG - Scalable Parallel Random Number Generator)
Time:    Wed May  3 12:40:13 2023
Kernel:  SSE2 - auto-detect threads (8 CPU cores detected)

Reading alignment file beetles_12s_data.fasta ... Fasta format detected
Alignment most likely contains DNA/RNA sequences
Alignment has 20 sequences with 352 columns, 106 distinct patterns
56 parsimony-informative, 51 singleton sites, 245 constant sites
                     Gap/Ambiguity  Composition  p-value
   1  G_viminalis_1          1.14%    passed     73.66%
   2  G_olivacea_1           1.14%    passed     92.86%
   3  G_rufipes              0.85%    passed     96.26%
   4  G_linnaeana            1.14%    passed     93.38%
   5  G_variabilis_1         0.85%    passed     94.67%
   6  G_fornicata            0.85%    passed     99.88%
   7  G_occidentalis         0.85%    passed     90.22%
   8  G_interposita_1        0.85%    passed     99.72%
   9  G_interposita_2        0.85%    passed     99.72%
  10  G_intermedia           0.85%    passed     99.99%
  11  G_quinquepunctata_2    0.85%    passed     99.99%
  12  G_holdausi             0.85%    passed     90.22%
  13  G_pallida_2            0.85%    passed     99.33%
  14  G_pallida_3            0.85%    passed     99.33%
  15  G_tredecimmaculata     0.57%    passed     93.87%
  16  G_nigropiagiata        0.85%    passed     79.05%
  17  G_kamikawai            0.85%    passed     99.51%
  18  G_rubripennis          0.85%    passed     81.32%
  19  Oreina_cacaiiae        0.57%    passed     96.74%
  20  Chrysomela_tremula     1.14%    passed     75.19%
****  TOTAL                  0.88%  0 sequences failed composition chi2 test (p-value<5%; df=3)
NOTE: G_interposita_2 is identical to G_interposita_1 but kept for subsequent analysis
NOTE: G_pallida_3 is identical to G_pallida_2 but kept for subsequent analysis


Create initial parsimony tree by phylogenetic likelihood library (PLL)... 0.002 seconds
NOTE: ModelFinder requires 1 MB RAM!
ModelFinder will test 286 DNA models (sample size: 352) ...
 No. Model         -LnL         df  AIC          AICc         BIC
Measuring multi-threading efficiency up to 8 CPU cores
Increase to 10 rounds for branch lengths
6447 trees examined
Threads: 1 / Time: 8.001 sec / Speedup: 1.000 / Efficiency: 100% / LogL: -2175
Threads: 2 / Time: 7.341 sec / Speedup: 1.090 / Efficiency: 54% / LogL: -2175
Threads: 3 / Time: 7.392 sec / Speedup: 1.082 / Efficiency: 36% / LogL: -2175
BEST NUMBER OF THREADS: 2

  1  JC            1677.783     37  3429.565     3438.521     3572.520
  2  JC+I          1616.115     38  3308.229     3317.699     3455.047
  3  JC+G4         1610.633     38  3297.265     3306.735     3444.083
  4  JC+I+G4       1608.440     39  3294.881     3304.881     3445.563
  5  JC+R2         1609.394     39  3296.788     3306.788     3447.470
  6  JC+R3         1608.823     41  3299.646     3310.756     3458.055
 14  F81+F         1580.487     40  3240.974     3251.520     3395.519
 15  F81+F+I       1512.490     41  3106.980     3118.090     3265.389
 16  F81+F+G4      1505.412     41  3092.824     3103.933     3251.233
 17  F81+F+I+G4    1502.921     42  3089.841     3101.531     3252.114
 18  F81+F+R2      1503.728     42  3091.456     3103.146     3253.729
 19  F81+F+R3      1503.250     44  3094.500     3107.399     3264.500
 27  K2P           1667.042     38  3410.084     3419.553     3556.902
 28  K2P+I         1605.083     39  3288.167     3298.167     3438.848
 29  K2P+G4        1599.700     39  3277.400     3287.400     3428.082
 30  K2P+I+G4      1597.591     40  3275.181     3285.728     3429.727
 31  K2P+R2        1598.490     40  3276.980     3287.527     3431.525
 32  K2P+R3        1597.835     42  3279.671     3291.360     3441.943
 40  HKY+F         1549.163     41  3180.326     3191.436     3338.735
 41  HKY+F+I       1473.868     42  3031.736     3043.425     3194.009
 42  HKY+F+G4      1463.805     42  3011.609     3023.298     3173.882
 43  HKY+F+I+G4    1462.182     43  3010.365     3022.651     3176.501
 44  HKY+F+R2      1463.797     43  3013.593     3025.879     3179.729
 45  HKY+F+R3      1463.155     45  3016.309     3029.839     3190.173
 53  TNe           1649.552     39  3377.104     3387.104     3527.786
 54  TNe+I         1585.319     40  3250.637     3261.184     3405.182
 55  TNe+G4        1580.937     40  3241.873     3252.420     3396.419
 56  TNe+I+G4      1579.743     41  3241.487     3252.596     3399.896
 57  TNe+R2        1581.487     41  3244.974     3256.084     3403.383
 58  TNe+R3        1580.964     43  3247.928     3260.214     3414.064
 66  TN+F          1543.835     42  3171.669     3183.359     3333.942
 67  TN+F+I        1468.833     43  3023.665     3035.951     3189.801
 68  TN+F+G4       1458.939     43  3003.878     3016.164     3170.014
 69  TN+F+I+G4     1457.384     44  3002.767     3015.666     3172.767
 70  TN+F+R2       1459.512     44  3007.023     3019.922     3177.023
 71  TN+F+R3       1457.746     46  3007.491     3021.668     3185.218
 79  K3P           1637.875     39  3353.751     3363.751     3504.433
 80  K3P+I         1575.284     40  3230.569     3241.115     3385.114
 81  K3P+G4        1569.514     40  3219.029     3229.575     3373.574
 82  K3P+I+G4      1567.447     41  3216.895     3228.004     3375.304
 83  K3P+R2        1568.130     41  3218.261     3229.370     3376.670
 84  K3P+R3        1565.924     43  3217.849     3230.135     3383.985
 92  K3Pu+F        1540.619     42  3165.238     3176.928     3327.511
 93  K3Pu+F+I      1467.515     43  3021.031     3033.316     3187.167
 94  K3Pu+F+G4     1458.695     43  3003.391     3015.677     3169.527
 95  K3Pu+F+I+G4   1457.017     44  3002.034     3014.933     3172.034
 96  K3Pu+F+R2     1457.930     44  3003.859     3016.758     3173.859
 97  K3Pu+F+R3     1455.775     46  3003.550     3017.727     3181.277
105  TPM2+F        1543.628     42  3171.255     3182.945     3333.528
106  TPM2+F+I      1470.518     43  3027.036     3039.321     3193.172
107  TPM2+F+G4     1461.266     43  3008.531     3020.817     3174.667
108  TPM2+F+I+G4   1459.369     44  3006.739     3019.638     3176.738
109  TPM2+F+R2     1460.451     44  3008.903     3021.802     3178.902
110  TPM2+F+R3     1457.898     46  3007.796     3021.973     3185.523
118  TPM2u+F       1543.628     42  3171.256     3182.945     3333.528
119  TPM2u+F+I     1470.518     43  3027.036     3039.321     3193.172
120  TPM2u+F+G4    1461.266     43  3008.532     3020.818     3174.668
121  TPM2u+F+I+G4  1459.367     44  3006.734     3019.633     3176.734
122  TPM2u+F+R2    1460.418     44  3008.836     3021.735     3178.835
123  TPM2u+F+R3    1457.766     46  3007.532     3021.709     3185.259
131  TPM3+F        1542.041     42  3168.083     3179.772     3330.355
132  TPM3+F+I      1468.182     43  3022.364     3034.650     3188.500
133  TPM3+F+G4     1459.266     43  3004.532     3016.818     3170.668
134  TPM3+F+I+G4   1457.666     44  3003.332     3016.231     3173.332
135  TPM3+F+R2     1458.540     44  3005.080     3017.979     3175.080
136  TPM3+F+R3     1456.144     46  3004.288     3018.465     3182.015
144  TPM3u+F       1542.042     42  3168.083     3179.773     3330.356
145  TPM3u+F+I     1468.182     43  3022.365     3034.650     3188.501
146  TPM3u+F+G4    1459.266     43  3004.532     3016.818     3170.668
147  TPM3u+F+I+G4  1457.664     44  3003.328     3016.227     3173.328
148  TPM3u+F+R2    1458.508     44  3005.016     3017.915     3175.015
149  TPM3u+F+R3    1456.104     46  3004.207     3018.384     3181.934
157  TIMe          1620.680     40  3321.359     3331.906     3475.905
158  TIMe+I        1555.840     41  3193.681     3204.790     3352.089
159  TIMe+G4       1550.967     41  3183.934     3195.044     3342.343
160  TIMe+I+G4     1549.870     42  3183.740     3195.430     3346.013
161  TIMe+R2       1551.192     42  3186.384     3198.073     3348.657
162  TIMe+R3       1550.052     44  3188.104     3201.003     3358.104
170  TIM+F         1535.387     43  3156.773     3169.059     3322.909
171  TIM+F+I       1462.444     44  3012.889     3025.788     3182.889
172  TIM+F+G4      1453.918     44  2995.837     3008.736     3165.837
173  TIM+F+I+G4    1452.327     45  2994.654     3008.183     3168.517
174  TIM+F+R2      1454.118     45  2998.237     3011.766     3172.100
175  TIM+F+R3      1451.919     47  2997.838     3012.680     3179.429
183  TIM2e         1623.531     40  3327.062     3337.609     3481.607
184  TIM2e+I       1560.950     41  3203.900     3215.009     3362.309
185  TIM2e+G4      1556.071     41  3194.142     3205.252     3352.551
186  TIM2e+I+G4    1554.161     42  3192.321     3204.010     3354.594
187  TIM2e+R2      1555.811     42  3195.623     3207.312     3357.895
188  TIM2e+R3      1552.257     44  3192.513     3205.412     3362.513
196  TIM2+F        1538.523     43  3163.046     3175.332     3329.182
197  TIM2+F+I      1465.317     44  3018.634     3031.533     3188.634
198  TIM2+F+G4     1455.963     44  2999.925     3012.824     3169.925
199  TIM2+F+I+G4   1454.211     45  2998.421     3011.951     3172.285
200  TIM2+F+R2     1456.605     45  3003.210     3016.739     3177.073
201  TIM2+F+R3     1453.649     47  3001.299     3016.141     3182.889
209  TIM3e         1631.002     40  3342.004     3352.550     3496.549
210  TIM3e+I       1566.406     41  3214.811     3225.921     3373.220
211  TIM3e+G4      1561.377     41  3204.754     3215.863     3363.163
212  TIM3e+I+G4    1560.322     42  3204.644     3216.334     3366.917
213  TIM3e+R2      1562.402     42  3208.804     3220.493     3371.077
214  TIM3e+R3      1560.910     44  3209.820     3222.719     3379.820
222  TIM3+F        1536.653     43  3159.306     3171.592     3325.442
223  TIM3+F+I      1463.148     44  3014.297     3027.196     3184.296
224  TIM3+F+G4     1454.728     44  2997.455     3010.354     3167.455
225  TIM3+F+I+G4   1453.224     45  2996.448     3009.977     3170.311
226  TIM3+F+R2     1454.893     45  2999.786     3013.316     3173.650
227  TIM3+F+R3     1452.867     47  2999.735     3014.577     3181.325
235  TVMe          1618.598     41  3319.196     3330.305     3477.605
236  TVMe+I        1557.038     42  3198.075     3209.765     3360.348
237  TVMe+G4       1550.093     42  3184.185     3195.875     3346.458
238  TVMe+I+G4     1547.241     43  3180.482     3192.767     3346.618
239  TVMe+R2       1548.268     43  3182.536     3194.821     3348.672
240  TVMe+R3       1542.901     45  3175.802     3189.331     3349.665
248  TVM+F         1536.157     44  3160.314     3173.213     3330.314
249  TVM+F+I       1464.542     45  3019.084     3032.614     3192.948
250  TVM+F+G4      1456.431     45  3002.862     3016.391     3176.725
251  TVM+F+I+G4    1454.567     46  3001.135     3015.312     3178.862
252  TVM+F+R2      1455.511     46  3003.022     3017.200     3180.750
253  TVM+F+R3      1452.978     48  3001.956     3017.480     3187.410
261  SYM           1600.934     42  3285.867     3297.556     3448.140
262  SYM+I         1538.011     43  3162.021     3174.307     3328.157
263  SYM+G4        1533.028     43  3152.056     3164.342     3318.192
264  SYM+I+G4      1531.381     44  3150.763     3163.662     3320.763
265  SYM+R2        1533.454     44  3154.908     3167.807     3324.908
266  SYM+R3        1530.582     46  3153.164     3167.341     3330.891
274  GTR+F         1530.983     45  3151.966     3165.495     3325.829
275  GTR+F+I       1459.349     46  3010.699     3024.876     3188.426
276  GTR+F+G4      1451.474     46  2994.947     3009.124     3172.674
277  GTR+F+I+G4    1449.785     47  2993.570     3008.412     3175.160
278  GTR+F+R2      1451.734     47  2997.468     3012.311     3179.059
279  GTR+F+R3      1449.248     49  2996.496     3012.721     3185.814
Akaike Information Criterion:           GTR+F+I+G4
Corrected Akaike Information Criterion: TIM+F+I+G4
Bayesian Information Criterion:         TIM+F+G4
Best-fit model: TIM+F+G4 chosen according to BIC

All model information printed to beetles_12s_data.fasta.model.gz
CPU time for ModelFinder: 45.721 seconds (0h:0m:45s)
Wall-clock time for ModelFinder: 23.666 seconds (0h:0m:23s)
Generating 1000 samples for ultrafast bootstrap (seed: 180988)...

NOTE: 0 MB RAM (0 GB) is required!
Measuring multi-threading efficiency up to 8 CPU cores
Increase to 10 rounds for branch lengths
2797 trees examined
Threads: 1 / Time: 8.002 sec / Speedup: 1.000 / Efficiency: 100% / LogL: -1942
Threads: 2 / Time: 5.371 sec / Speedup: 1.490 / Efficiency: 74% / LogL: -1942
Threads: 3 / Time: 4.923 sec / Speedup: 1.625 / Efficiency: 54% / LogL: -1942
Threads: 4 / Time: 5.456 sec / Speedup: 1.467 / Efficiency: 37% / LogL: -1942
BEST NUMBER OF THREADS: 3

Estimate model parameters (epsilon = 0.100)
1. Initial log-likelihood: -1531.886
2. Current log-likelihood: -1456.310
3. Current log-likelihood: -1454.023
Optimal log-likelihood: -1453.920
Rate parameters:  A-C: 1.00000  A-G: 5.44270  A-T: 2.96594  C-G: 2.96594  C-T: 13.60827  G-T: 1.00000
Base frequencies:  A: 0.422  C: 0.135  G: 0.066  T: 0.377
Gamma shape alpha: 0.234
Parameters optimization took 3 rounds (0.006 sec)
Computing ML distances based on estimated model parameters... 0.004 sec
Computing BIONJ tree...
0.001 seconds
Log-likelihood of BIONJ tree: -1454.865
--------------------------------------------------------------------
|             INITIALIZING CANDIDATE TREE SET                      |
--------------------------------------------------------------------
Generating 98 parsimony trees... 0.049 second
Computing log-likelihood of 98 initial trees ... 0.126 seconds
Current best score: -1453.301

Do NNI search on 20 best initial trees
Estimate model parameters (epsilon = 0.100)
BETTER TREE FOUND at iteration 1: -1453.182
UPDATE BEST LOG-LIKELIHOOD: -1453.182
Iteration 10 / LogL: -1453.191 / Time: 0h:0m:24s
Iteration 20 / LogL: -1453.984 / Time: 0h:0m:24s
Finish initializing candidate tree set (5)
Current best tree score: -1453.182 / CPU time: 0.343
Number of iterations: 20
--------------------------------------------------------------------
|               OPTIMIZING CANDIDATE TREE SET                      |
--------------------------------------------------------------------
UPDATE BEST LOG-LIKELIHOOD: -1453.181
UPDATE BEST LOG-LIKELIHOOD: -1453.180
Iteration 30 / LogL: -1453.180 / Time: 0h:0m:24s (0h:0m:59s left)
Iteration 40 / LogL: -1453.181 / Time: 0h:0m:24s (0h:0m:38s left)
Iteration 50 / LogL: -1458.565 / Time: 0h:0m:24s (0h:0m:25s left)
Log-likelihood cutoff on original alignment: -1472.644
Iteration 60 / LogL: -1453.646 / Time: 0h:0m:24s (0h:0m:17s left)
Iteration 70 / LogL: -1454.821 / Time: 0h:0m:24s (0h:0m:11s left)
Iteration 80 / LogL: -1453.378 / Time: 0h:0m:25s (0h:0m:6s left)
Iteration 90 / LogL: -1453.181 / Time: 0h:0m:25s (0h:0m:3s left)
Iteration 100 / LogL: -1454.821 / Time: 0h:0m:25s (0h:0m:0s left)
Log-likelihood cutoff on original alignment: -1474.255
NOTE: Bootstrap correlation coefficient of split occurrence frequencies: 0.996
UPDATE BEST LOG-LIKELIHOOD: -1453.180
TREE SEARCH COMPLETED AFTER 102 ITERATIONS / Time: 0h:0m:25s

--------------------------------------------------------------------
|                    FINALIZING TREE SEARCH                        |
--------------------------------------------------------------------
Performs final model parameters optimization
Estimate model parameters (epsilon = 0.010)
1. Initial log-likelihood: -1453.180
Optimal log-likelihood: -1453.180
Rate parameters:  A-C: 1.00000  A-G: 6.44918  A-T: 3.37365  C-G: 3.37365  C-T: 15.71030  G-T: 1.00000
Base frequencies:  A: 0.422  C: 0.135  G: 0.066  T: 0.377
Gamma shape alpha: 0.233
Parameters optimization took 1 rounds (0.008 sec)
BEST SCORE FOUND : -1453.180
Creating bootstrap support values...
Split supports printed to NEXUS file beetles_12s_data.fasta.splits.nex
Total tree length: 0.874

Total number of iterations: 102
CPU time used for tree search: 4.679 sec (0h:0m:4s)
Wall-clock time used for tree search: 1.731 sec (0h:0m:1s)
Total CPU time used: 60.090 sec (0h:1m:0s)
Total wall-clock time used: 25.554 sec (0h:0m:25s)

Computing bootstrap consensus tree...
Reading input file beetles_12s_data.fasta.splits.nex...
20 taxa and 170 splits.
Consensus tree written to beetles_12s_data.fasta.contree
Reading input trees file beetles_12s_data.fasta.contree
Log-likelihood of consensus tree: -1453.664

Analysis results written to: 
  IQ-TREE report:                beetles_12s_data.fasta.iqtree
  Maximum-likelihood tree:       beetles_12s_data.fasta.treefile
  Likelihood distances:          beetles_12s_data.fasta.mldist

Ultrafast bootstrap approximation results written to:
  Split support values:          beetles_12s_data.fasta.splits.nex
  Consensus tree:                beetles_12s_data.fasta.contree
  Screen log file:               beetles_12s_data.fasta.log

Date and Time: Wed May  3 12:41:02 2023
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git add .                                
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git commit -m "updated files and folders"
[master 264953f] updated files and folders
 Committer: Aidyn Kehrli <aidynkehrli@Aidyns-MacBook-Pro.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 15 files changed, 936 insertions(+), 20 deletions(-)
 create mode 100644 beetles_12s_data.fasta.bionj
 create mode 100644 beetles_12s_data.fasta.ckp.gz
 create mode 100644 beetles_12s_data.fasta.contree
 create mode 100644 beetles_12s_data.fasta.iqtree
 create mode 100644 beetles_12s_data.fasta.log
 create mode 100644 beetles_12s_data.fasta.mldist
 create mode 100644 beetles_12s_data.fasta.model.gz
 create mode 100644 beetles_12s_data.fasta.splits.nex
 create mode 100644 beetles_12s_data.fasta.treefile
 create mode 100644 iqtree-1.6.12-MacOSX/bin/beetles_12s_data.fasta.log
 create mode 100644 iqtree-1.6.12-MacOSX/bin/beetles_12s_data.fasta.log.log
 create mode 100644 iqtree-1.6.12-MacOSX/bin/beetles_12s_data.log
 create mode 100644 iqtree-1.6.12-MacOSX/bin/beetles_12s_data.log.log
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git push
Enumerating objects: 24, done.
Counting objects: 100% (24/24), done.
Delta compression using up to 8 threads
Compressing objects: 100% (19/19), done.
Writing objects: 100% (19/19), 49.04 KiB | 16.35 MiB/s, done.
Total 19 (delta 7), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (7/7), completed with 4 local objects.
To https://github.com/aidynkehrli/Botany-563.git
   2b8b5e6..264953f  master -> master
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % pwd                                      
/Users/aidynkehrli/Desktop/Botany-563
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % ./iqtree -s beetles_16s_data.fasta -bb 1000 -nt AUTO
IQ-TREE multicore version 1.6.12 for Mac OS X 64-bit built Aug 15 2019
Developed by Bui Quang Minh, Nguyen Lam Tung, Olga Chernomor,
Heiko Schmidt, Dominik Schrempf, Michael Woodhams.

Host:    Aidyns-MacBook-Pro.local (SSE4.2, 8 GB RAM)
Command: ./iqtree -s beetles_16s_data.fasta -bb 1000 -nt AUTO
Seed:    335129 (Using SPRNG - Scalable Parallel Random Number Generator)
Time:    Wed May  3 12:43:46 2023
Kernel:  SSE2 - auto-detect threads (8 CPU cores detected)

Reading alignment file beetles_16s_data.fasta ... Fasta format detected
Alignment most likely contains DNA/RNA sequences
Alignment has 20 sequences with 486 columns, 156 distinct patterns
106 parsimony-informative, 58 singleton sites, 322 constant sites
                    Gap/Ambiguity  Composition  p-value
   1  G_viminalis_1         1.65%    passed     99.86%
   2  G_olivacea_1          1.85%    passed     97.04%
   3  G_rufipes             2.67%    passed     99.85%
   4  G_linnaeana           1.23%    passed     99.91%
   5  G_variabilis_1        1.44%    passed     94.46%
   6  G_fornicata           1.44%    passed     98.31%
   7  G_occidentalis        2.47%    passed     99.66%
   8  G_interposita_1       1.65%    passed     95.94%
   9  G_interposita_2       1.65%    passed     95.94%
  10  G_intermedia          1.65%    passed     99.90%
  11  G_quinquepunctata     2.06%    passed     96.97%
  12  G_holdausi            2.26%    passed     99.38%
  13  G_pallida_2           1.85%    passed     98.61%
  14  G_pallida_3           1.85%    passed     98.44%
  15  G_tredecimmaculata    3.50%    passed     97.17%
  16  G_nigropiagiata       3.29%    passed     97.85%
  17  G_kamikawai           1.23%    passed     98.75%
  18  G_rubripennis         1.23%    passed     99.55%
  19  Oreina                1.85%    passed     86.34%
  20  Chrysomela            3.09%    passed     88.79%
****  TOTAL                 2.00%  0 sequences failed composition chi2 test (p-value<5%; df=3)
NOTE: G_interposita_2 is identical to G_interposita_1 but kept for subsequent analysis


Create initial parsimony tree by phylogenetic likelihood library (PLL)... 0.001 seconds
NOTE: ModelFinder requires 1 MB RAM!
ModelFinder will test 286 DNA models (sample size: 486) ...
 No. Model         -LnL         df  AIC          AICc         BIC
Measuring multi-threading efficiency up to 8 CPU cores
Increase to 10 rounds for branch lengths
5375 trees examined
Threads: 1 / Time: 8.001 sec / Speedup: 1.000 / Efficiency: 100% / LogL: -3104
Threads: 2 / Time: 6.490 sec / Speedup: 1.233 / Efficiency: 62% / LogL: -3104
Threads: 3 / Time: 6.311 sec / Speedup: 1.268 / Efficiency: 42% / LogL: -3104
BEST NUMBER OF THREADS: 2

  1  JC            2543.472     37  5160.943     5167.220     5315.833
  2  JC+I          2439.801     38  4955.603     4962.234     5114.679
  3  JC+G4         2427.243     38  4930.486     4937.117     5089.562
  4  JC+I+G4       2425.664     39  4929.327     4936.323     5092.589
  5  JC+R2         2424.478     39  4926.957     4933.952     5090.219
  6  JC+R3         2424.203     41  4930.406     4938.163     5102.041
 14  F81+F         2401.430     40  4882.861     4890.232     5050.309
 15  F81+F+I       2281.565     41  4645.129     4652.886     4816.764
 16  F81+F+G4      2265.197     41  4612.393     4620.150     4784.028
 17  F81+F+I+G4    2261.843     42  4607.687     4615.840     4783.507
 18  F81+F+R2      2260.784     42  4605.569     4613.722     4781.390
 19  F81+F+R3      2260.129     44  4608.257     4617.237     4792.450
 27  K2P           2543.435     38  5162.870     5169.500     5321.946
 28  K2P+I         2439.754     39  4957.508     4964.503     5120.770
 29  K2P+G4        2427.208     39  4932.417     4939.412     5095.679
 30  K2P+I+G4      2425.628     40  4931.255     4938.626     5098.704
 31  K2P+R2        2424.315     40  4928.630     4936.001     5096.078
 32  K2P+R3        2424.101     42  4932.202     4940.355     5108.022
 40  HKY+F         2396.189     41  4874.379     4882.136     5046.013
 41  HKY+F+I       2271.132     42  4626.265     4634.418     4802.085
 42  HKY+F+G4      2253.614     42  4591.229     4599.382     4767.050
 43  HKY+F+I+G4    2249.954     43  4585.908     4594.469     4765.915
 44  HKY+F+R2      2250.123     43  4586.245     4594.806     4766.252
 45  HKY+F+R3      2246.590     45  4583.181     4592.590     4771.560
 53  TNe           2521.346     39  5120.691     5127.687     5283.953
 54  TNe+I         2415.306     40  4910.613     4917.983     5078.061
 55  TNe+G4        2403.559     40  4887.117     4894.488     5054.566
 56  TNe+I+G4      2402.720     41  4887.439     4895.196     5059.074
 57  TNe+R2        2402.292     41  4886.584     4894.341     5058.218
 58  TNe+R3        2402.169     43  4890.337     4898.898     5070.344
 66  TN+F          2387.101     42  4858.203     4866.356     5034.024
 67  TN+F+I        2261.699     43  4609.399     4617.960     4789.406
 68  TN+F+G4       2245.643     43  4577.286     4585.847     4757.293
 69  TN+F+I+G4     2242.093     44  4572.185     4581.165     4756.378
 70  TN+F+R2       2244.022     44  4576.043     4585.023     4760.236
 71  TN+F+R3       2239.349     46  4570.697     4580.547     4763.263
 79  K3P           2488.601     39  5055.202     5062.198     5218.464
 80  K3P+I         2381.996     40  4843.992     4851.363     5011.440
 81  K3P+G4        2369.005     40  4818.011     4825.381     4985.459
 82  K3P+I+G4      2367.285     41  4816.569     4824.326     4988.204
 83  K3P+R2        2366.042     41  4814.085     4821.841     4985.719
 84  K3P+R3        2366.043     43  4818.086     4826.647     4998.093
 92  K3Pu+F        2373.631     42  4831.262     4839.415     5007.083
 93  K3Pu+F+I      2256.783     43  4599.567     4608.128     4779.574
 94  K3Pu+F+G4     2240.785     43  4567.570     4576.131     4747.577
 95  K3Pu+F+I+G4   2237.615     44  4563.230     4572.210     4747.424
 96  K3Pu+F+R2     2236.558     44  4561.115     4570.095     4745.308
 97  K3Pu+F+R3     2236.544     46  4565.087     4574.937     4757.653
105  TPM2+F        2381.438     42  4846.876     4855.030     5022.697
106  TPM2+F+I      2262.572     43  4611.145     4619.706     4791.152
107  TPM2+F+G4     2247.298     43  4580.597     4589.158     4760.604
108  TPM2+F+I+G4   2243.720     44  4575.439     4584.419     4759.632
109  TPM2+F+R2     2243.480     44  4574.960     4583.940     4759.154
110  TPM2+F+R3     2243.478     46  4578.956     4588.805     4771.521
118  TPM2u+F       2381.436     42  4846.873     4855.026     5022.693
119  TPM2u+F+I     2262.571     43  4611.142     4619.703     4791.149
120  TPM2u+F+G4    2247.297     43  4580.594     4589.155     4760.601
121  TPM2u+F+I+G4  2243.710     44  4575.420     4584.400     4759.613
122  TPM2u+F+R2    2243.473     44  4574.946     4583.925     4759.139
123  TPM2u+F+R3    2243.469     46  4578.938     4588.788     4771.504
131  TPM3+F        2376.125     42  4836.251     4844.404     5012.072
132  TPM3+F+I      2259.941     43  4605.882     4614.443     4785.889
133  TPM3+F+G4     2242.626     43  4571.252     4579.813     4751.259
134  TPM3+F+I+G4   2239.644     44  4567.287     4576.267     4751.480
135  TPM3+F+R2     2238.287     44  4564.574     4573.553     4748.767
136  TPM3+F+R3     2238.280     46  4568.561     4578.410     4761.126
144  TPM3u+F       2376.126     42  4836.251     4844.405     5012.072
145  TPM3u+F+I     2259.940     43  4605.880     4614.441     4785.887
146  TPM3u+F+G4    2242.626     43  4571.252     4579.813     4751.259
147  TPM3u+F+I+G4  2239.643     44  4567.287     4576.266     4751.480
148  TPM3u+F+R2    2238.280     44  4564.560     4573.539     4748.753
149  TPM3u+F+R3    2238.277     46  4568.554     4578.404     4761.120
157  TIMe          2466.565     40  5013.131     5020.502     5180.579
158  TIMe+I        2357.543     41  4797.085     4804.842     4968.720
159  TIMe+G4       2345.123     41  4772.246     4780.003     4943.880
160  TIMe+I+G4     2344.075     42  4772.149     4780.303     4947.970
161  TIMe+R2       2343.750     42  4771.500     4779.654     4947.321
162  TIMe+R3       2343.735     44  4775.470     4784.450     4959.664
170  TIM+F         2364.647     43  4815.294     4823.855     4995.301
171  TIM+F+I       2247.287     44  4582.575     4591.554     4766.768
172  TIM+F+G4      2232.380     44  4552.760     4561.739     4736.953
173  TIM+F+I+G4    2229.539     45  4549.077     4558.486     4737.456
174  TIM+F+R2      2230.072     45  4550.144     4559.553     4738.523
175  TIM+F+R3      2230.063     47  4554.127     4564.428     4750.878
183  TIM2e         2466.579     40  5013.159     5020.530     5180.607
184  TIM2e+I       2363.933     41  4809.866     4817.623     4981.501
185  TIM2e+G4      2350.794     41  4783.588     4791.345     4955.223
186  TIM2e+I+G4    2349.479     42  4782.957     4791.111     4958.778
187  TIM2e+R2      2348.533     42  4781.067     4789.220     4956.888
188  TIM2e+R3      2348.532     44  4785.065     4794.044     4969.258
196  TIM2+F        2372.823     43  4831.646     4840.207     5011.653
197  TIM2+F+I      2252.162     44  4592.324     4601.304     4776.517
198  TIM2+F+G4     2237.235     44  4562.471     4571.450     4746.664
199  TIM2+F+I+G4   2234.026     45  4558.052     4567.461     4746.431
200  TIM2+F+R2     2235.936     45  4561.872     4571.282     4750.252
201  TIM2+F+R3     2235.892     47  4565.784     4576.085     4762.535
209  TIM3e         2480.607     40  5041.214     5048.585     5208.662
210  TIM3e+I       2382.715     41  4847.429     4855.186     5019.064
211  TIM3e+G4      2368.105     41  4818.211     4825.967     4989.845
212  TIM3e+I+G4    2367.876     42  4819.752     4827.906     4995.573
213  TIM3e+R2      2367.440     42  4818.879     4827.033     4994.700
214  TIM3e+R3      2367.431     44  4822.861     4831.841     5007.055
222  TIM3+F        2366.694     43  4819.387     4827.948     4999.394
223  TIM3+F+I      2250.652     44  4589.304     4598.283     4773.497
224  TIM3+F+G4     2235.082     44  4558.163     4567.143     4742.356
225  TIM3+F+I+G4   2232.354     45  4554.708     4564.117     4743.087
226  TIM3+F+R2     2232.437     45  4554.874     4564.283     4743.254
227  TIM3+F+R3     2232.402     47  4558.804     4569.105     4755.556
235  TVMe          2441.445     41  4964.890     4972.647     5136.525
236  TVMe+I        2344.974     42  4773.948     4782.101     4949.768
237  TVMe+G4       2329.054     42  4742.109     4750.262     4917.929
238  TVMe+I+G4     2327.789     43  4741.578     4750.139     4921.585
239  TVMe+R2       2326.251     43  4738.503     4747.064     4918.510
240  TVMe+R3       2326.251     45  4742.502     4751.911     4930.881
248  TVM+F         2361.406     44  4810.812     4819.791     4995.005
249  TVM+F+I       2251.084     45  4592.169     4601.578     4780.548
250  TVM+F+G4      2235.857     45  4561.714     4571.123     4750.093
251  TVM+F+I+G4    2232.943     46  4557.886     4567.735     4750.451
252  TVM+F+R2      2231.338     46  4554.675     4564.525     4747.241
253  TVM+F+R3      2231.319     48  4558.637     4569.402     4759.575
261  SYM           2419.662     42  4923.324     4931.478     5099.145
262  SYM+I         2322.363     43  4730.726     4739.287     4910.733
263  SYM+G4        2308.080     43  4702.161     4710.722     4882.167
264  SYM+I+G4      2307.377     44  4702.754     4711.734     4886.947
265  SYM+R2        2306.329     44  4700.658     4709.638     4884.851
266  SYM+R3        2306.329     46  4704.658     4714.507     4897.223
274  GTR+F         2352.472     45  4794.945     4804.354     4983.324
275  GTR+F+I       2240.847     46  4573.693     4583.543     4766.259
276  GTR+F+G4      2226.370     46  4544.739     4554.589     4737.305
277  GTR+F+I+G4    2223.965     47  4541.931     4552.232     4738.683
278  GTR+F+R2      2224.062     47  4542.123     4552.425     4738.875
279  GTR+F+R3      2224.035     49  4546.070     4557.308     4751.194
Akaike Information Criterion:           GTR+F+I+G4
Corrected Akaike Information Criterion: GTR+F+I+G4
Bayesian Information Criterion:         TIM+F+G4
Best-fit model: TIM+F+G4 chosen according to BIC

All model information printed to beetles_16s_data.fasta.model.gz
CPU time for ModelFinder: 42.298 seconds (0h:0m:42s)
Wall-clock time for ModelFinder: 21.645 seconds (0h:0m:21s)
Generating 1000 samples for ultrafast bootstrap (seed: 335129)...

NOTE: 1 MB RAM (0 GB) is required!
Measuring multi-threading efficiency up to 8 CPU cores
Increase to 10 rounds for branch lengths
2175 trees examined
Threads: 1 / Time: 8.000 sec / Speedup: 1.000 / Efficiency: 100% / LogL: -2779
Threads: 2 / Time: 5.031 sec / Speedup: 1.590 / Efficiency: 80% / LogL: -2779
Threads: 3 / Time: 4.353 sec / Speedup: 1.838 / Efficiency: 61% / LogL: -2779
Threads: 4 / Time: 4.637 sec / Speedup: 1.725 / Efficiency: 43% / LogL: -2779
BEST NUMBER OF THREADS: 3

Estimate model parameters (epsilon = 0.100)
1. Initial log-likelihood: -2311.302
2. Current log-likelihood: -2234.911
3. Current log-likelihood: -2232.422
Optimal log-likelihood: -2232.380
Rate parameters:  A-C: 1.00000  A-G: 2.02092  A-T: 3.08883  C-G: 3.08883  C-T: 6.27754  G-T: 1.00000
Base frequencies:  A: 0.405  C: 0.159  G: 0.082  T: 0.355
Gamma shape alpha: 0.256
Parameters optimization took 3 rounds (0.011 sec)
Computing ML distances based on estimated model parameters... 0.004 sec
Computing BIONJ tree...
0.000 seconds
Log-likelihood of BIONJ tree: -2230.656
--------------------------------------------------------------------
|             INITIALIZING CANDIDATE TREE SET                      |
--------------------------------------------------------------------
Generating 98 parsimony trees... 0.054 second
Computing log-likelihood of 98 initial trees ... 0.143 seconds
Current best score: -2230.566

Do NNI search on 20 best initial trees
Estimate model parameters (epsilon = 0.100)
BETTER TREE FOUND at iteration 1: -2229.449
Iteration 10 / LogL: -2229.456 / Time: 0h:0m:22s
Iteration 20 / LogL: -2229.496 / Time: 0h:0m:22s
Finish initializing candidate tree set (1)
Current best tree score: -2229.449 / CPU time: 0.401
Number of iterations: 20
--------------------------------------------------------------------
|               OPTIMIZING CANDIDATE TREE SET                      |
--------------------------------------------------------------------
Iteration 30 / LogL: -2229.618 / Time: 0h:0m:22s (0h:0m:55s left)
Iteration 40 / LogL: -2232.469 / Time: 0h:0m:22s (0h:0m:35s left)
Iteration 50 / LogL: -2232.084 / Time: 0h:0m:23s (0h:0m:23s left)
Log-likelihood cutoff on original alignment: -2256.576
Iteration 60 / LogL: -2232.084 / Time: 0h:0m:23s (0h:0m:16s left)
Iteration 70 / LogL: -2232.478 / Time: 0h:0m:23s (0h:0m:10s left)
Iteration 80 / LogL: -2232.084 / Time: 0h:0m:23s (0h:0m:6s left)
Iteration 90 / LogL: -2232.661 / Time: 0h:0m:23s (0h:0m:2s left)
Iteration 100 / LogL: -2229.493 / Time: 0h:0m:23s (0h:0m:0s left)
Log-likelihood cutoff on original alignment: -2256.135
NOTE: Bootstrap correlation coefficient of split occurrence frequencies: 0.982
NOTE: UFBoot does not converge, continue at least 100 more iterations
Iteration 110 / LogL: -2229.495 / Time: 0h:0m:24s (0h:0m:19s left)
Iteration 120 / LogL: -2232.469 / Time: 0h:0m:24s (0h:0m:16s left)
Iteration 130 / LogL: -2232.084 / Time: 0h:0m:24s (0h:0m:13s left)
Iteration 140 / LogL: -2229.460 / Time: 0h:0m:24s (0h:0m:10s left)
Iteration 150 / LogL: -2232.084 / Time: 0h:0m:24s (0h:0m:8s left)
Log-likelihood cutoff on original alignment: -2255.651
Iteration 160 / LogL: -2232.084 / Time: 0h:0m:24s (0h:0m:6s left)
Iteration 170 / LogL: -2232.457 / Time: 0h:0m:25s (0h:0m:4s left)
Iteration 180 / LogL: -2232.084 / Time: 0h:0m:25s (0h:0m:2s left)
Iteration 190 / LogL: -2232.708 / Time: 0h:0m:25s (0h:0m:1s left)
Iteration 200 / LogL: -2232.661 / Time: 0h:0m:25s (0h:0m:0s left)
Log-likelihood cutoff on original alignment: -2255.651
NOTE: Bootstrap correlation coefficient of split occurrence frequencies: 0.999
TREE SEARCH COMPLETED AFTER 200 ITERATIONS / Time: 0h:0m:25s

--------------------------------------------------------------------
|                    FINALIZING TREE SEARCH                        |
--------------------------------------------------------------------
Performs final model parameters optimization
Estimate model parameters (epsilon = 0.010)
1. Initial log-likelihood: -2229.449
Optimal log-likelihood: -2229.449
Rate parameters:  A-C: 1.00000  A-G: 2.15599  A-T: 3.24054  C-G: 3.24054  C-T: 6.66709  G-T: 1.00000
Base frequencies:  A: 0.405  C: 0.159  G: 0.082  T: 0.355
Gamma shape alpha: 0.257
Parameters optimization took 1 rounds (0.002 sec)
BEST SCORE FOUND : -2229.449
Creating bootstrap support values...
Split supports printed to NEXUS file beetles_16s_data.fasta.splits.nex
Total tree length: 1.037

Total number of iterations: 200
CPU time used for tree search: 10.437 sec (0h:0m:10s)
Wall-clock time used for tree search: 3.816 sec (0h:0m:3s)
Total CPU time used: 59.954 sec (0h:0m:59s)
Total wall-clock time used: 25.908 sec (0h:0m:25s)

Computing bootstrap consensus tree...
Reading input file beetles_16s_data.fasta.splits.nex...
20 taxa and 207 splits.
Consensus tree written to beetles_16s_data.fasta.contree
Reading input trees file beetles_16s_data.fasta.contree
Log-likelihood of consensus tree: -2229.449

Analysis results written to: 
  IQ-TREE report:                beetles_16s_data.fasta.iqtree
  Maximum-likelihood tree:       beetles_16s_data.fasta.treefile
  Likelihood distances:          beetles_16s_data.fasta.mldist

Ultrafast bootstrap approximation results written to:
  Split support values:          beetles_16s_data.fasta.splits.nex
  Consensus tree:                beetles_16s_data.fasta.contree
  Screen log file:               beetles_16s_data.fasta.log

Date and Time: Wed May  3 12:44:33 2023
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git add .
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git commit "updated files and folders"
error: pathspec 'updated files and folders' did not match any file(s) known to git
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git commit -m "updated files and folders"
[master 87c11d7] updated files and folders
 Committer: Aidyn Kehrli <aidynkehrli@Aidyns-MacBook-Pro.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 10 files changed, 935 insertions(+), 20 deletions(-)
 create mode 100644 beetles_16s_data.fasta.bionj
 create mode 100644 beetles_16s_data.fasta.ckp.gz
 create mode 100644 beetles_16s_data.fasta.contree
 create mode 100644 beetles_16s_data.fasta.iqtree
 create mode 100644 beetles_16s_data.fasta.log
 create mode 100644 beetles_16s_data.fasta.mldist
 create mode 100644 beetles_16s_data.fasta.model.gz
 create mode 100644 beetles_16s_data.fasta.splits.nex
 create mode 100644 beetles_16s_data.fasta.treefile
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git commit
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git push
Enumerating objects: 14, done.
Counting objects: 100% (14/14), done.
Delta compression using up to 8 threads
Compressing objects: 100% (12/12), done.
Writing objects: 100% (12/12), 48.52 KiB | 16.17 MiB/s, done.
Total 12 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/aidynkehrli/Botany-563.git
   264953f..87c11d7  master -> master
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git add .
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git commit -m "updated files and folders"
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % git push
Everything up-to-date
(base) aidynkehrli@Aidyns-MacBook-Pro Botany-563 % 
