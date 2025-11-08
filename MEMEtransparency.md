# Bionformatics-Lab-MEME

N2 gene

Last login: Wed Oct 29 05:16:28 on ttys000

(base) fred@192 ~ % conda config --add channels conda-forge

Warning: 'conda-forge' already in 'channels' list, moving to the top

(base) fred@192 ~ % conda config --add channels bioconda

Warning: 'bioconda' already in 'channels' list, moving to the top

(base) fred@192 ~ % conda config --set channel_priority strict

(base) fred@192 ~ % conda install hyphy

2 channel Terms of Service accepted

Channels:

 - bioconda

 - conda-forge

 - defaults

Platform: osx-arm64

Collecting package metadata (repodata.json): done

Solving environment: done

==> WARNING: A newer version of conda exists. <==

    current version: 25.7.0

    latest version: 25.9.1

Please update conda by running

    $ conda update -n base -c conda-forge conda

## Package Plan ##

  environment location: /opt/anaconda3

  added / updated specs:

    - hyphy

The following packages will be downloaded:

    package                    |            build

    ---------------------------|-----------------

    hyphy-2.5.64               |       hafd6872_0         3.3 MB  bioconda

    libcxx-21.1.4              |       hf598326_0         555 KB  conda-forge

    libgfortran-5.0.0          |14_2_0_h6c33f7e_103         153 KB  conda-forge

    libgfortran5-14.2.0        |     h6c33f7e_103         788 KB  conda-forge

    libzlib-1.2.13             |       hfb2fe0b_6          46 KB  conda-forge

    llvm-openmp-21.1.4         |       h4a912ad_0         279 KB  conda-forge

    zlib-1.2.13                |       hfb2fe0b_6          76 KB  conda-forge

    ------------------------------------------------------------

                                           Total:         5.2 MB

The following NEW packages will be INSTALLED:

  hyphy              bioconda/osx-arm64::hyphy-2.5.64-hafd6872_0 

  libzlib            conda-forge/osx-arm64::libzlib-1.2.13-hfb2fe0b_6 

  mpi                conda-forge/osx-arm64::mpi-1.0-openmpi 

  openmpi            conda-forge/osx-arm64::openmpi-4.1.6-h526c993_101 

The following packages will be UPDATED:

  libcxx                pkgs/main::libcxx-14.0.6-h848a8c0_0 --> conda-forge::libcxx-21.1.4-hf598326_0 

  libgfortran        pkgs/main::libgfortran-5.0.0-11_3_0_h~ --> conda-forge::libgfortran-5.0.0-14_2_0_h6c33f7e_103 

  libgfortran5       pkgs/main::libgfortran5-11.3.0-h00934~ --> conda-forge::libgfortran5-14.2.0-h6c33f7e_103 

  llvm-openmp        pkgs/main::llvm-openmp-14.0.6-hc6e570~ --> conda-forge::llvm-openmp-21.1.4-h4a912ad_0 

  zlib                    pkgs/main::zlib-1.2.13-h18a0788_1 --> conda-forge::zlib-1.2.13-hfb2fe0b_6 

Proceed ([y]/n)? y

Downloading and Extracting Packages:

                                                                                

Preparing transaction: done                                                     

Verifying transaction: done                                                     

Executing transaction: done                                                     

(base) fred@192 ~ % hyphy i-

Error:

Could not read batch file '/Users/fred/i-'.

Path stack:

	/opt/anaconda3/share/hyphy/

	/Users/fred/

Check errors.log for execution error details.

(base) fred@192 ~ % hyphy i-

Error:

Could not read batch file '/Users/fred/i-'.

Path stack:

	/opt/anaconda3/share/hyphy/

	/Users/fred/

Check errors.log for execution error details.

(base) fred@192 ~ % source ~/.bash_profile

(base) fred@192 ~ % conda activate /opt/miniconda3/envs/paml_env

(paml_env) fred@192 ~ % cd ~/Downloads

(paml_env) fred@192 Downloads % hyphy -i

HYPHY 2.5.84(MP) for Darwin on arm64 ARM Neon SIMD zlib (v1.3.1)

***************** TYPES OF STANDARD ANALYSES *****************

	(1) Selection Analyses

	(2) Evolutionary Hypothesis Testing

	(3) Relative evolutionary rate inference

	(4) Coevolutionary analysis

	(5) Basic Analyses

	(6) Codon Selection Analyses

	(7) Compartmentalization

	(8) Data File Tools

	(9) Tree File Tools

	(10) Miscellaneous

	(11) Model Comparison

	(12) Molecular Clock

	(13) Phylogeny Reconstruction

	(14) Positive Selection

	(15) Recombination

	(16) Selection/Recombination

	(17) Relative Rate

	(18) Relative Ratio

 Please select type of analyses you want to list (or press ENTER to process custom batch file):1

***************** FILES IN 'Selection Analyses' ***************** 

	(1) [MEME] Test for episodic site-level selection using MEME (Mixed Effects Model of Evolution).

	(2) [FEL] Test for pervasive site-level selection using FEL (Fixed Effects Likelihood).

	(3) [SLAC] Test for pervasive site-level selection using SLAC (Single Likelihood Ancestor Counting).

	(4) [FUBAR] Test for pervasive site-level selection using FUBAR (Fast Unconstrained Bayesian AppRoximation for inferring selection).

	(5) [BUSTED] Test for episodic gene-wide selection using BUSTED (Branch-site Unrestricted Statistical Test of Episodic Diversification).

	(6) [aBSREL] Test for lineage-specific evolution using the branch-site method aBS-REL (Adaptive Branch-Site Random Effects Likelihood).

	(7) [RELAX] Test for relaxation of selection pressure along a specified set of test branches using RELAX (a random effects test of selection relaxation).

	(8) [FADE] Test a protein alignment for directional selection towards specific amino acids along a specified set of test branches using FADE (a FUBAR Approach to Directional Evolution).

	(9) [PRIME] 

	(10) [Error-Filter] Use a BUSTED-E model fit to clean-up a sequence alignment

	(11)  "[MSS] Fits a model with multiple synonymous rates (MSS model) to several genes jointly."

	(12)  "[MSS-GA] Perform a Genetic Algorithm search model selection for a codon MSS model on a collection of alignments."

	(13)  "[MSS-GA-processor] Process results for a genetic algorithm codon MSS model search."

	(14) [BUSTED-PH] Test if episodic diversifying selection is associated with the set of designated (FG) branches using BUSTED (Branch-site Unrestricted Statistical Test of Episodic Diversification).

 Please select the analysis you would like to perform (or press ENTER to return to the list of analysis types):1

Analysis Description

--------------------

MEME (Mixed Effects Model of Evolution) estimates a site-wise synonymous

(&alpha;) and a two-category mixture of non-synonymous (&beta;-, with

Multiple partitions within a NEXUS file are also supported for

recombination - aware analysis. Version 3.0 adds a different format for

ancestral state reconstruction, branch-site posterior storage, and

site-level heterogeneity testing. Version 4 adds support for multiple

hits and more than 2 rate classes on omega, as well as site-level

imputation option. Version 4.1 fixes bugs with EBF computation for > 2

more rates and MH reporting. 

proportion p-, and &beta;+ with proportion [1-p-]) rates, and uses a

likelihood ratio test to determine if &beta;+ > &alpha; at a site. The

estimates aggregate information over a proportion of branches at a site,

so the signal is derived from episodic diversification, which is a

combination of strength of selection [effect size] and the proportion of

the tree affected. A subset of branches can be selected for testing as

well, in which case an additional (nuisance) parameter will be inferred

-- the non-synonymous rate on branches NOT selected for testing.

- __Requirements__: in-frame codon alignment and a phylogenetic tree

- __Citation__: Detecting Individual Sites Subject to Episodic Diversifying Selection.

_PLoS Genet_ 8(7): e1002764.

- __Written by__: Sergei L. Kosakovsky Pond, Steven Weaver

- __Contact Information__: spond@temple.edu

- __Analysis Version__: 4.1

####Choose Genetic Code

1. [**Universal**] Universal code. (Genebank transl_table=1).

2. [**Vertebrate-mtDNA**] Vertebrate mitochondrial DNA code. (Genebank transl_table=2).

3. [**Yeast-mtDNA**] Yeast mitochondrial DNA code. (Genebank transl_table=3).

4. [**Mold-Protozoan-mtDNA**] Mold, Protozoan and Coelenterate mitochondrial DNA and the Mycloplasma/Spiroplasma code. (Genebank transl_table=4).

5. [**Invertebrate-mtDNA**] Invertebrate mitochondrial DNA code. (Genebank transl_table=5).

6. [**Ciliate-Nuclear**] Ciliate, Dasycladacean and Hexamita Nuclear code. (Genebank transl_table=6).

7. [**Echinoderm-mtDNA**] Echinoderm mitochondrial DNA code. (Genebank transl_table=9).

8. [**Euplotid-Nuclear**] Euplotid Nuclear code. (Genebank transl_table=10).

9. [**Alt-Yeast-Nuclear**] Alternative Yeast Nuclear code. (Genebank transl_table=12).

10. [**Ascidian-mtDNA**] Ascidian mitochondrial DNA code. (Genebank transl_table=13).

11. [**Flatworm-mtDNA**] Flatworm mitochondrial DNA code. (Genebank transl_table=14).

12. [**Blepharisma-Nuclear**] Blepharisma Nuclear code. (Genebank transl_table=15).

13. [**Chlorophycean-mtDNA**] Chlorophycean Mitochondrial Code (transl_table=16).

14. [**Trematode-mtDNA**] Trematode Mitochondrial Code (transl_table=21).

15. [**Scenedesmus-obliquus-mtDNA**] Scenedesmus obliquus mitochondrial Code (transl_table=22).

16. [**Thraustochytrium-mtDNA**] Thraustochytrium Mitochondrial Code (transl_table=23).

17. [**Pterobranchia-mtDNA**] Pterobranchia Mitochondrial Code (transl_table=24).

18. [**SR1-and-Gracilibacteria**] Candidate Division SR1 and Gracilibacteria Code (transl_table=25).

19. [**Pachysolen-Nuclear**] Pachysolen tannophilus Nuclear Code (transl_table=26).

20. [**Mesodinium-Nuclear**] Mesodinium Nuclear Code (transl_table=29)

21. [**Peritrich-Nuclear**] Peritrich Nuclear Code (transl_table=30)

22. [**Cephalodiscidae-mtDNA**] Cephalodiscidae Mitochondrial UAA-Tyr Code (transl_table=33)

>Please choose an option (or press q to cancel selection):1

>Select a coding sequence alignment file (`/Users/fred/Downloads/`) N2_master_TRIMMED.fas

-------

>[WARNING] '/Users/fred/Downloads/N2_master_TRIMMED.fas' contains 1

duplicate sequence. Identical sequences do not contribute any

information to the analysis and only slow down computation. Please

consider removing duplicate or 'nearly' duplicate sequences, e.g. using

https://github.com/veg/hyphy-analyses/tree/master/remove-duplicates

prior to running selection analyses

-------

>Please select a tree file for the data: (`/Users/fred/Downloads/`) N2_FINAL.tree

/Users/fred/Downloads/N2_FINAL.tree

N2_FINAL.tree

>Loaded a multiple sequence alignment with **620** sequences, **1238** codons, and **1** partitions from `/Users/fred/Downloads/N2_master_TRIMMED.fas`

####Choose the set of branches to test for selection

1. [**All**] Include all branches in the analysis

2. [**Internal**] Include all internal branches in the analysis

3. [**Leaves**] Include all leaf branches in the analysis

4. [**Unlabeled branches**] Set of 1237 unlabeled branches

>Please choose an option (or press q to cancel selection):1

>Select the p-value threshold to use when testing for selection (permissible range = [0,1], default value = 0.1): 0.1

>[Advanced setting, will result in MUCH SLOWER run time] Perform parametric bootstrap resampling to derive site-level null LRT distributions up to this many replicates per site. Recommended use for small to medium (<30 sequences) datasets (permissible range = [0,1000], default value = 50, integer): 

Error:

Could not read all the parameters requested. in call to fscanf(stdin,"String",str_val);

Function call stack

1 :  [namespace = Wu_FKvGY] fscanf(stdin,"String",str_val);

-------

2 :  meme.resample=io.PromptUser("\n>[Advanced setting, will result in MUCH SLOWER run time] Perform parametric bootstrap resampling to derive site-level null LRT distributions up to this many replicates per site. Recommended use for small to medium (<30 sequences) datasets",50,0,1000,TRUE);

-------

Check errors.log for execution error details.

(paml_env) fred@192 Downloads % 0

zsh: command not found: 0

(paml_env) fred@192 Downloads % hyphy /opt/miniconda3/envs/paml_env/share/hyphy/selection/FEL.bf --alignment N2_master_TRIMMED.fas --tree N2_FINAL.tree --output FEL_results.json --srv 0 --p-value 0.1

Error:

Could not read batch file '/opt/miniconda3/envs/paml_env/share/hyphy/selection/FEL.bf'.

Path stack:

	/opt/miniconda3/envs/paml_env/share/hyphy/

	/opt/miniconda3/envs/paml_env/share/hyphy/selection/

Check errors.log for execution error details.

(paml_env) fred@192 Downloads % hyphy i-

Error:

Could not read batch file '/Users/fred/Downloads/i-'.

Path stack:

	/opt/miniconda3/envs/paml_env/share/hyphy/

	/Users/fred/Downloads/

Check errors.log for execution error details.

(paml_env) fred@192 Downloads % hyphy -i

HYPHY 2.5.84(MP) for Darwin on arm64 ARM Neon SIMD zlib (v1.3.1)

***************** TYPES OF STANDARD ANALYSES *****************

	(1) Selection Analyses

	(2) Evolutionary Hypothesis Testing

	(3) Relative evolutionary rate inference

	(4) Coevolutionary analysis

	(5) Basic Analyses

	(6) Codon Selection Analyses

	(7) Compartmentalization

	(8) Data File Tools

	(9) Tree File Tools

	(10) Miscellaneous

	(11) Model Comparison

	(12) Molecular Clock

	(13) Phylogeny Reconstruction

	(14) Positive Selection

	(15) Recombination

	(16) Selection/Recombination

	(17) Relative Rate

	(18) Relative Ratio

 Please select type of analyses you want to list (or press ENTER to process custom batch file):1

***************** FILES IN 'Selection Analyses' ***************** 

	(1) [MEME] Test for episodic site-level selection using MEME (Mixed Effects Model of Evolution).

	(2) [FEL] Test for pervasive site-level selection using FEL (Fixed Effects Likelihood).

	(3) [SLAC] Test for pervasive site-level selection using SLAC (Single Likelihood Ancestor Counting).

	(4) [FUBAR] Test for pervasive site-level selection using FUBAR (Fast Unconstrained Bayesian AppRoximation for inferring selection).

	(5) [BUSTED] Test for episodic gene-wide selection using BUSTED (Branch-site Unrestricted Statistical Test of Episodic Diversification).

	(6) [aBSREL] Test for lineage-specific evolution using the branch-site method aBS-REL (Adaptive Branch-Site Random Effects Likelihood).

	(7) [RELAX] Test for relaxation of selection pressure along a specified set of test branches using RELAX (a random effects test of selection relaxation).

	(8) [FADE] Test a protein alignment for directional selection towards specific amino acids along a specified set of test branches using FADE (a FUBAR Approach to Directional Evolution).

	(9) [PRIME] 

	(10) [Error-Filter] Use a BUSTED-E model fit to clean-up a sequence alignment

	(11)  "[MSS] Fits a model with multiple synonymous rates (MSS model) to several genes jointly."

	(12)  "[MSS-GA] Perform a Genetic Algorithm search model selection for a codon MSS model on a collection of alignments."

	(13)  "[MSS-GA-processor] Process results for a genetic algorithm codon MSS model search."

	(14) [BUSTED-PH] Test if episodic diversifying selection is associated with the set of designated (FG) branches using BUSTED (Branch-site Unrestricted Statistical Test of Episodic Diversification).

 Please select the analysis you would like to perform (or press ENTER to return to the list of analysis types):1

Analysis Description

--------------------

MEME (Mixed Effects Model of Evolution) estimates a site-wise synonymous

(&alpha;) and a two-category mixture of non-synonymous (&beta;-, with

Multiple partitions within a NEXUS file are also supported for

recombination - aware analysis. Version 3.0 adds a different format for

ancestral state reconstruction, branch-site posterior storage, and

site-level heterogeneity testing. Version 4 adds support for multiple

hits and more than 2 rate classes on omega, as well as site-level

imputation option. Version 4.1 fixes bugs with EBF computation for > 2

more rates and MH reporting. 

proportion p-, and &beta;+ with proportion [1-p-]) rates, and uses a

likelihood ratio test to determine if &beta;+ > &alpha; at a site. The

estimates aggregate information over a proportion of branches at a site,

so the signal is derived from episodic diversification, which is a

combination of strength of selection [effect size] and the proportion of

the tree affected. A subset of branches can be selected for testing as

well, in which case an additional (nuisance) parameter will be inferred

-- the non-synonymous rate on branches NOT selected for testing.

- __Requirements__: in-frame codon alignment and a phylogenetic tree

- __Citation__: Detecting Individual Sites Subject to Episodic Diversifying Selection.

_PLoS Genet_ 8(7): e1002764.

- __Written by__: Sergei L. Kosakovsky Pond, Steven Weaver

- __Contact Information__: spond@temple.edu

- __Analysis Version__: 4.1

####Choose Genetic Code

1. [**Universal**] Universal code. (Genebank transl_table=1).

2. [**Vertebrate-mtDNA**] Vertebrate mitochondrial DNA code. (Genebank transl_table=2).

3. [**Yeast-mtDNA**] Yeast mitochondrial DNA code. (Genebank transl_table=3).

4. [**Mold-Protozoan-mtDNA**] Mold, Protozoan and Coelenterate mitochondrial DNA and the Mycloplasma/Spiroplasma code. (Genebank transl_table=4).

5. [**Invertebrate-mtDNA**] Invertebrate mitochondrial DNA code. (Genebank transl_table=5).

6. [**Ciliate-Nuclear**] Ciliate, Dasycladacean and Hexamita Nuclear code. (Genebank transl_table=6).

7. [**Echinoderm-mtDNA**] Echinoderm mitochondrial DNA code. (Genebank transl_table=9).

8. [**Euplotid-Nuclear**] Euplotid Nuclear code. (Genebank transl_table=10).

9. [**Alt-Yeast-Nuclear**] Alternative Yeast Nuclear code. (Genebank transl_table=12).

10. [**Ascidian-mtDNA**] Ascidian mitochondrial DNA code. (Genebank transl_table=13).

11. [**Flatworm-mtDNA**] Flatworm mitochondrial DNA code. (Genebank transl_table=14).

12. [**Blepharisma-Nuclear**] Blepharisma Nuclear code. (Genebank transl_table=15).

13. [**Chlorophycean-mtDNA**] Chlorophycean Mitochondrial Code (transl_table=16).

14. [**Trematode-mtDNA**] Trematode Mitochondrial Code (transl_table=21).

15. [**Scenedesmus-obliquus-mtDNA**] Scenedesmus obliquus mitochondrial Code (transl_table=22).

16. [**Thraustochytrium-mtDNA**] Thraustochytrium Mitochondrial Code (transl_table=23).

17. [**Pterobranchia-mtDNA**] Pterobranchia Mitochondrial Code (transl_table=24).

18. [**SR1-and-Gracilibacteria**] Candidate Division SR1 and Gracilibacteria Code (transl_table=25).

19. [**Pachysolen-Nuclear**] Pachysolen tannophilus Nuclear Code (transl_table=26).

20. [**Mesodinium-Nuclear**] Mesodinium Nuclear Code (transl_table=29)

21. [**Peritrich-Nuclear**] Peritrich Nuclear Code (transl_table=30)

22. [**Cephalodiscidae-mtDNA**] Cephalodiscidae Mitochondrial UAA-Tyr Code (transl_table=33)

>Please choose an option (or press q to cancel selection):1

>Select a coding sequence alignment file (`/Users/fred/Downloads/`) N2_master_TRIMMED.fas

-------

>[WARNING] '/Users/fred/Downloads/N2_master_TRIMMED.fas' contains 1

duplicate sequence. Identical sequences do not contribute any

information to the analysis and only slow down computation. Please

consider removing duplicate or 'nearly' duplicate sequences, e.g. using

https://github.com/veg/hyphy-analyses/tree/master/remove-duplicates

prior to running selection analyses

-------

>Please select a tree file for the data: (`/Users/fred/Downloads/`) N2_FINAL.tree

/Users/fred/Downloads/N2_FINAL.tree

N2_FINAL.tree

>Loaded a multiple sequence alignment with **620** sequences, **1238** codons, and **1** partitions from `/Users/fred/Downloads/N2_master_TRIMMED.fas`

####Choose the set of branches to test for selection

1. [**All**] Include all branches in the analysis

2. [**Internal**] Include all internal branches in the analysis

3. [**Leaves**] Include all leaf branches in the analysis

4. [**Unlabeled branches**] Set of 1237 unlabeled branches

>Please choose an option (or press q to cancel selection):1

>Select the p-value threshold to use when testing for selection (permissible range = [0,1], default value = 0.1): 0.1

>[Advanced setting, will result in MUCH SLOWER run time] Perform parametric bootstrap resampling to derive site-level null LRT distributions up to this many replicates per site. Recommended use for small to medium (<30 sequences) datasets (permissible range = [0,1000], default value = 50, integer): 50

The number omega rate classes to include in the model [2 is the strongly recommended default] (permissible range = [2,4], default value = 2, integer): 2

####Include support for multiple nucleotide substitutions

1. [**Double**] Include branch-specific rates for double nucleotide substitutions

2. [**Double+Triple**] Include branch-specific rates for double and triple nucleotide substitutions

3. [**None**] [Default] Use standard models which permit only single nucleotide changes to occur instantly

>Please choose an option (or press q to cancel selection):3

####Impute likely states for sequences

1. [**Yes**] Impute marginal likelihoods for each codon at each sequence and each site

2. [**No**] Do not impute marginal likelihoods for each codon at each sequence and each site

>Please choose an option (or press q to cancel selection):2

####Optimization precision settings for preliminary fits

1. [**standard**] [Default] Use standard optimization settings.

2. [**reduced**] Cruder optimizations settings for faster fitting of preliminary models

>Please choose an option (or press q to cancel selection):1

>Save the resulting JSON file to (`/Users/fred/Downloads/`) MEME_results.json

### Branches to include in the MEME analysis

Selected 1237 branches to include in the MEME analysis: `seq448, seq366, seq414, seq27, seq391, Node8, Node6, seq96, seq430, Node11, Node5, Node3, Node1, seq514, seq420, seq213, seq266, Node22, Node20, seq271, seq402, seq443, Node28, Node26, seq293, Node25, Node19, seq55, seq579, Node34, seq455, seq194, seq107, seq219, Node42, Node40, Node38, seq305, seq582, Node45, Node37, Node33, seq355, seq508, Node50, seq502, seq104, seq159, Node55, Node53, Node49, seq115, seq178, seq287, Node64, Node62, seq491, seq585, Node67, Node61, seq174, seq316, seq441, Node79, seq286, seq202, seq372, Node91, seq396, seq490, seq125, Node100, seq77, seq413, Node105, seq390, seq187, Node108, Node104, seq608, seq207, seq578, Node114, Node112, seq384, seq453, Node117, Node111, Node103, Node99, Node97, seq601, seq20, Node120, Node96, seq30, Node95, seq57, seq614, Node124, Node94, Node90, seq418, Node89, seq435, seq49, seq169, Node131, Node129, seq298, Node128, Node88, Node86, seq101, Node85, seq276, seq303, seq429, Node139, seq67, seq83, Node142, Node138, Node136, Node84, seq88, seq292, seq119, seq181, Node152, Node150, seq496, seq594, Node155, Node149, Node147, seq108, seq163, Node159, seq513, seq43, seq212, seq70, Node168, Node166, Node164, seq505, Node163, seq37, seq95, Node172, Node162, Node158, Node146, seq379, seq528, seq136, seq25, Node179, Node177, Node175, Node145, Node83, seq360, seq367, seq157, seq133, seq472, Node190, Node188, Node186, Node184, seq519, seq586, seq113, seq460, Node199, Node197, seq222, seq310, Node203, seq61, seq191, Node206, Node202, Node196, Node194, seq407, seq447, Node210, seq218, seq425, Node213, Node209, Node193, Node183, seq270, seq15, seq466, Node218, Node216, Node182, Node82, Node78, Node76, seq199, seq267, seq171, seq438, Node231, seq463, seq32, seq204, Node239, seq93, Node238, seq313, Node237, Node235, seq363, seq126, seq155, seq469, Node249, Node247, Node245, seq86, seq492, seq589, seq177, seq117, seq289, Node261, Node259, Node257, Node255, Node253, seq487, seq64, seq17, Node274, Node272, seq449, Node271, seq97, seq416, seq28, seq393, Node285, Node283, seq432, Node282, Node280, seq369, Node279, seq382, seq522, Node290, Node278, Node270, seq301, seq454, Node293, Node269, seq58, seq581, Node297, seq220, seq112, seq196, Node303, Node301, seq457, seq306, seq596, Node308, Node306, Node300, Node296, Node268, seq273, seq404, seq444, Node316, Node314, seq422, seq11, seq21, seq279, Node323, Node321, Node319, Node313, seq295, Node312, seq375, seq80, seq410, seq73, seq605, Node336, Node334, Node332, seq283, Node331, Node329, seq51, Node328, seq121, seq185, seq602, Node343, Node341, Node327, Node311, Node267, seq516, Node266, seq46, seq166, Node349, seq387, seq399, Node352, Node348, seq507, seq102, seq161, Node358, seq510, seq357, seq501, seq617, Node366, seq190, seq40, seq210, Node372, Node370, seq69, seq498, Node375, Node369, Node365, Node363, Node361, Node357, Node355, Node347, Node265, seq215, seq479, seq611, seq134, seq529, Node384, Node382, Node380, Node378, Node264, Node252, Node244, Node234, Node230, Node228, seq575, Node227, Node225, seq484, Node224, seq480, Node223, seq483, seq349, seq570, seq474, seq264, seq6, seq332, seq538, Node411, Node409, seq238, seq330, Node415, seq254, seq242, seq145, Node421, Node419, seq328, Node418, Node414, Node408, Node406, Node404, seq7, seq234, seq248, seq540, Node431, Node429, seq151, seq232, Node435, seq230, seq592, Node438, Node434, Node428, seq139, seq597, seq326, seq568, Node449, Node447, seq240, seq476, Node454, seq246, seq550, Node457, Node453, seq546, Node452, Node446, seq340, seq260, seq236, Node464, Node462, seq262, seq318, Node468, seq536, Node467, Node461, Node445, seq336, seq324, seq5, seq141, seq255, seq346, seq554, Node485, seq322, seq562, Node488, Node484, Node482, Node480, Node478, Node476, Node474, seq320, seq258, seq227, seq147, Node495, Node493, Node491, Node473, seq552, Node472, Node444, seq149, seq250, seq348, seq143, seq556, Node505, Node503, Node501, Node499, Node443, Node441, Node427, Node425, Node403, seq534, seq544, seq338, seq566, Node513, Node511, Node509, seq532, seq341, seq344, seq252, seq547, seq564, seq244, seq352, Node528, Node526, Node524, Node522, Node520, Node518, Node516, Node508, Node402, Node400, seq572, seq334, seq354, Node533, Node531, Node399, seq542, Node398, seq560, Node397, seq558, Node396, Node394, seq571, seq333, seq353, Node543, Node541, seq263, seq335, Node553, seq345, seq553, Node560, seq561, seq321, Node563, Node559, seq256, Node558, seq4, Node557, seq323, seq140, Node568, Node556, Node552, seq257, seq319, seq146, seq228, Node576, Node574, Node572, seq233, seq595, seq325, seq567, Node586, Node584, seq261, seq317, Node589, Node583, Node581, seq235, seq545, seq239, seq475, Node601, seq245, seq549, Node604, Node600, Node598, seq551, Node597, seq259, Node596, seq249, seq347, seq142, seq555, Node614, Node612, seq148, Node611, Node609, Node595, seq339, Node594, Node592, Node580, seq535, Node579, Node571, Node551, seq533, seq543, seq337, seq565, Node625, Node623, Node621, seq8, Node620, Node550, seq138, Node549, seq569, Node548, seq559, Node547, seq541, Node546, Node540, seq343, seq251, seq548, seq243, seq351, seq563, Node642, Node640, Node638, Node636, Node634, seq342, seq223, seq473, Node648, Node646, seq531, seq224, seq226, seq225, Node656, Node654, Node652, seq144, seq253, seq241, Node663, seq331, seq537, Node667, seq327, seq237, seq329, Node672, Node670, Node666, Node662, Node660, seq247, seq539, Node676, seq150, seq231, seq350, Node682, Node680, seq590, seq229, seq557, Node687, Node685, Node679, Node675, Node659, Node651, Node645, Node633, Node539, Node393, Node391, seq315, seq94, seq365, seq471, seq129, seq154, Node701, Node699, Node697, Node695, seq376, seq489, seq619, seq42, seq192, seq71, Node721, Node719, Node717, seq82, Node716, seq66, Node715, Node713, Node711, seq406, seq446, Node726, Node710, seq518, seq304, seq275, seq309, seq383, seq524, Node744, seq297, Node743, Node741, seq123, seq100, seq31, seq394, Node753, Node751, seq434, seq3, Node758, seq412, Node757, seq209, Node756, Node750, Node748, Node740, seq75, seq606, Node764, seq452, Node763, Node739, seq285, seq419, Node768, Node738, seq18, seq280, Node771, Node737, seq13, seq54, Node774, Node736, Node734, seq371, Node733, Node731, Node729, Node709, seq459, seq584, Node780, seq111, seq221, Node783, Node779, seq59, Node778, Node708, seq2, seq1, Node787, Node707, seq359, seq47, seq168, Node793, seq389, seq401, Node796, Node792, Node790, Node706, seq89, seq291, seq118, seq179, Node804, seq495, seq593, Node807, Node803, Node801, Node799, Node705, seq175, seq440, Node812, seq465, seq506, Node815, Node811, seq268, Node810, Node704, Node694, seq35, seq512, seq105, seq162, Node825, Node823, Node821, seq216, seq424, Node829, seq613, seq137, seq530, Node834, Node832, Node828, Node820, seq201, seq577, Node837, Node819, Node693, Node691, seq493, seq85, seq478, seq203, seq462, seq33, seq311, Node853, Node851, Node849, Node847, seq172, seq437, Node857, seq265, seq214, seq131, seq526, Node864, Node862, Node860, Node856, Node846, seq91, seq574, seq56, seq580, Node875, seq456, seq307, seq583, Node881, Node879, seq109, seq193, Node884, Node878, Node874, seq486, seq409, seq74, seq604, Node894, Node892, Node890, seq23, seq277, Node898, seq610, Node897, Node889, seq374, seq197, seq450, Node906, Node904, seq52, seq385, seq398, Node914, seq45, seq165, Node917, Node913, seq294, seq380, seq520, Node922, Node920, Node912, seq368, seq184, seq599, Node928, seq26, seq392, Node934, seq282, seq415, Node937, Node933, seq98, Node932, seq431, Node931, Node927, Node925, Node911, Node909, Node903, seq300, seq427, Node943, seq62, seq616, seq182, seq39, seq211, seq500, Node956, Node954, Node952, Node950, Node948, seq78, Node947, seq16, Node946, Node942, Node902, Node888, seq515, seq421, seq10, seq122, Node966, seq272, seq403, seq442, Node972, Node970, seq152, Node969, Node965, Node963, Node961, Node887, Node873, seq356, seq503, seq509, seq103, seq158, Node982, Node980, Node978, Node976, Node872, Node870, seq362, seq128, seq468, Node987, Node985, Node869, Node867, Node845, Node843, Node841, seq587, seq176, seq114, seq288, Node994, Node992, Node990, Node840, Node690, Node390, Node222, seq290, seq116, seq180, Node1003, Node1001, seq87, seq494, seq591, Node1008, Node1006, Node1000, seq173, seq439, Node1013, seq314, seq517, Node1017, seq504, seq405, seq445, Node1024, seq458, seq110, seq195, Node1030, Node1028, seq308, seq588, Node1033, Node1027, Node1023, Node1021, seq364, seq470, seq130, seq156, Node1041, Node1039, Node1037, seq411, seq76, seq607, Node1049, Node1047, seq423, seq217, Node1052, Node1046, seq377, seq612, seq135, seq527, Node1059, Node1057, Node1055, Node1045, seq481, seq106, seq160, Node1064, Node1062, Node1044, Node1036, Node1020, Node1016, Node1012, seq65, seq274, Node1070, seq302, seq428, Node1073, Node1069, seq12, seq600, seq186, Node1083, Node1081, seq370, Node1080, seq29, seq395, Node1090, seq284, seq417, Node1093, Node1089, seq99, Node1088, seq433, Node1087, Node1079, seq48, seq167, Node1100, seq388, seq400, Node1103, Node1099, seq60, seq381, seq523, Node1108, Node1106, Node1098, Node1078, seq200, seq488, seq189, seq41, seq618, Node1118, Node1116, Node1114, Node1112, seq19, seq451, Node1121, Node1111, Node1077, seq206, seq24, Node1126, seq124, Node1125, seq53, seq81, Node1130, Node1124, Node1076, Node1068, seq358, seq511, Node1134, seq296, seq36, seq92, Node1139, Node1137, Node1133, Node1067, Node1011, Node999, seq269, seq576, Node1142, Node998, seq464, Node997, Node221, Node75, seq482, Node74, seq461, Node73, seq312, Node72, seq436, seq198, seq573, Node1152, Node1150, seq170, Node1149, Node71, seq34, seq620, Node1158, seq90, Node1157, seq361, seq127, seq153, Node1165, seq84, seq467, Node1168, Node1164, Node1162, Node1156, Node70, Node60, seq477, seq525, seq132, seq609, Node1175, Node1173, Node1171, Node59, seq408, seq72, seq79, seq603, Node1184, Node1182, Node1180, seq63, seq485, Node1188, seq281, seq22, seq278, Node1195, Node1193, seq188, seq497, seq615, seq499, Node1203, Node1201, Node1199, seq68, seq38, seq208, Node1208, Node1206, Node1198, Node1192, seq373, Node1191, Node1187, Node1179, seq205, seq50, seq183, seq598, Node1217, seq9, seq120, Node1220, Node1216, Node1214, Node1212, Node1178, Node58, Node48, Node32, Node18, Node16, seq14, seq299, seq426, Node1225, Node1223, Node15, seq378, seq521, Node1228, Node14, seq44, seq164, Node1232, seq386, seq397, Node1235, Node1231`

### Obtaining branch lengths and nucleotide substitution biases under the nucleotide GTR model

>Use/Save parameter estimates from 'initial-guess' model fits (`/Users/fred/Downloads/`) null

    

####Reduce zero-length branches

1. [**Yes**] Automatically delete internal zero-length branches for computational efficiency (will not affect results otherwise)

2. [**Constrain**] Keep zero-length branches, but constrain their values to 0

3. [**No**] Keep all branches

>Please choose an option (or press q to cancel selection):

1. [**Yes**] Automatically delete internal zero-length branches for computational efficiency (will not affect results otherwise)

2. [**Constrain**] Keep zero-length branches, but constrain their values to 0

3. [**No**] Keep all branches

>Please choose an option (or press q to cancel selection):1

### Deleted 106 zero-length internal branches: `Node1, Node1003, Node103, Node1041, Node108, Node1080, Node1083, Node1088, Node1112, Node1118, Node112, Node1121, Node1124, Node1125, Node1130, Node1182, Node1191, Node1201, Node1203, Node1206, Node1208, Node128, Node145, Node152, Node155, Node162, Node163, Node168, Node179, Node194, Node199, Node202, Node206, Node237, Node238, Node239, Node270, Node274, Node278, Node282, Node303, Node361, Node370, Node375, Node414, Node418, Node434, Node444, Node446, Node462, Node467, Node472, Node473, Node480, Node484, Node488, Node501, Node556, Node558, Node563, Node581, Node583, Node592, Node594, Node595, Node596, Node611, Node64, Node642, Node679, Node709, Node715, Node716, Node721, Node729, Node734, Node737, Node738, Node739, Node740, Node748, Node750, Node756, Node757, Node763, Node771, Node804, Node810, Node853, Node887, Node89, Node90, Node912, Node932, Node933, Node94, Node947, Node95, Node952, Node954, Node956, Node96, Node969, Node97, Node99, Node998`

* Log(L) = -78293.82, AIC-c = 159078.99 (1245 estimated parameters)

* 1 partition. Total tree length by partition (subs/site) 43.867

### Obtaining the global omega estimate based on relative GTR branch lengths and nucleotide substitution biases

* Log(L) = -74528.70, AIC-c = 151352.82 (1146 estimated parameters)

* 1 partition. Total tree length by partition (subs/site) 50.061

* non-synonymous/synonymous rate ratio for *test* =   0.2033

####Perform branch length re-optimization under the full codon model

1. [**Yes**] [Default] Perform branch length re-optimization under the full codon model

2. [**No**] Skip branch length re-optimization under the full codon model (faster but less precise)

>Please choose an option (or press q to cancel selection):1

Only analyze sites whose 1-based indices match the following list (null to skip) : null

For sites whose 1-based indices match the following list, write out likelihood function snapshots (null string to skip) : null string

### Improving branch lengths, nucleotide substitution biases, and global dN/dS ratios under a full codon model

* Log(L) = -74105.61

* Log(L) = -74105.61, AIC-c = 150506.65 (1146 estimated parameters)

* 1 partition. Total tree length by partition (subs/site) 74.079

* non-synonymous/synonymous rate ratio for *test* =   0.1452
### For partition 1 these sites are significant at p <=0.1

|   Codon    | Partition  |   alpha    |non-syn rate (beta) distribution, rates : weights|    LRT     |Episodic selection detected?| # branches |         List of most common codon substitutions at this site          |

|:----------:|:----------:|:----------:|:-----------------------------------------------:|:----------:|:--------------------------:|:----------:|:---------------------------------------------------------------------:|

|     34     |     1      |    4.976   |            1.16/23099.19 : 1.00/0.00            |   12.746   |      Yes, p =  0.0196      |     1      |[67]Agc>Ngc|[51]CAa>NNa|[33]CAg>NNg|[7]AGc>NNc|[3]aaT>aaC,Agt>Ngt|[2...|

|     36     |     1      |   11.290   |            0.16/23154.65 : 0.89/0.11            |   58.434   |      Yes, p =  0.0196      |     10     |[7]AtC>CtA|[2]acA>acC,acA>acG,atC>atA,cTC>cNN|[1]acA>acT,atA>atC,Atg...|

|     42     |     1      |    4.011   |             0.72/280.78 : 0.60/0.40             |    3.236   |      Yes, p =  0.0980      |     6      |[66]Aca>Nca|[11]Gac>Nac|[9]Aac>Nac|[7]Acg>Ncg|[3]aGc>aAc,AGc>NAc|[2]...|

|    183     |     1      |    6.057   |             0.00/53.79 : 0.79/0.21              |    1.654   |      Yes, p =  0.0980      |     1      |                          [1]GAc>AGc,gaC>gaT                           |

|    209     |     1      |   24.660   |             0.00/796.65 : 0.85/0.15             |    3.197   |      Yes, p =  0.0784      |     0      |[56]TTc>NNc|[3]TTC>NNT|[2]CTc>NNc,ttC>ttT,TTt>NNt,ttT>ttC|[1]TTc>AGc...|

|    243     |     1      |    8.462   |             0.46/28.14 : 0.92/0.08              |    1.855   |      Yes, p =  0.0588      |     2      |[148]Gaa>Naa|[76]Caa>Naa|[65]ggC>ggN|[6]Gag>Nag|[5]Cag>Nag|[4]GgC>Ng...|

|    283     |     1      |    4.144   |             0.64/68.70 : 0.69/0.31              |    1.758   |      Yes, p =  0.0392      |     1      |[70]AGa>NNa|[57]AAc>NNc|[10]Gaa>Naa|[4]AAa>NNa|[2]acC>acA,acC>acN|[1...|

|    285     |     1      |   11.002   |             0.29/56.36 : 0.80/0.20              |    1.831   |      Yes, p =  0.0588      |     6      |[78]gtC>gtN|[48]gTG>gNN|[4]aTG>aNN,gcG>gcN,gtC>gtT,gtT>gtC|[2]Aca>Gc...|

|    356     |     1      |    0.758   |             0.64/43.89 : 0.01/0.99              |    9.047   |      Yes, p =  0.0196      |     1      |[77]atC>atN|[64]AcA>NcN|[61]aTT>aNN|[20]ccC>ccN|[11]ctC>ctN|[6]Aca>N...|

|    359     |     1      |    2.821   |             0.00/10.11 : 0.86/0.14              |    3.647   |      Yes, p =  0.0980      |     12     |[82]tGG>tNN|[79]aTA>aNN|[17]aTC>aNN|[5]aGa>aAa|[4]gTa>gCa|[2]atC>atT...|

|    368     |     1      |    4.448   |             0.79/27.96 : 0.91/0.09              |    1.064   |      Yes, p =  0.0588      |     0      |[76]Aca>Nca|[75]ATt>NNt|[73]aTG>aNN|[10]AGg>NNg|[4]gaA>gaG|[3]aTG>aC...|

|    373     |     1      |   12.245   |             0.99/97.09 : 0.89/0.11              |    1.354   |      Yes, p =  0.0784      |     1      |[5]agT>agC|[3]agA>agG,ggA>ggG,ggG>ggA|[2]AAa>GGa,aTG>aCA,Gga>Aga|[1]...|

|    443     |     1      |   13.032   |             1.02/555.64 : 0.91/0.09             |    5.182   |      Yes, p =  0.0392      |     2      |[30]aaG>aaN|[4]aaG>aaA,caA>caG|[3]cgA>cgG|[2]acC>acT,tgC>tgT|[1]aaA>...|

|    445     |     1      |    5.508   |             2.15/74.25 : 0.92/0.08              |    2.574   |      Yes, p =  0.0588      |     1      |[78]Gtt>Ntt|[70]cAC>cNN|[39]tGG>tNN|[33]cGG>cNN|[5]tAC>tNN|[4]aAc>aG...|

|    446     |     1      |    5.612   |             0.37/116.17 : 0.82/0.18             |    5.712   |      Yes, p =  0.0196      |     4      |[79]gTC>gNN|[78]tCG>tNN|[75]Ttg>Ntg|[73]cTC>cNN|[3]atC>atT|[2]cCG>cN...|

|    461     |     1      |    5.799   |             0.07/24.28 : 0.78/0.22              |    2.159   |      Yes, p =  0.0980      |     5      |[78]Ccc>Ncc|[74]ccA>ccN|[29]Act>Nct|[3]ccA>ccC,ccA>ccG,ccG>ccA|[2]Ac...|

|    474     |     1      |    5.310   |             0.69/97.93 : 0.89/0.11              |    3.619   |      Yes, p =  0.0196      |     2      |[75]gTA>gNN|[65]aTG>aNN|[3]aAA>aNN|[2]aaA>aaG,aTG>aAA,tcT>tcC,tCt>tT...|

|    571     |     1      |    7.084   |             1.60/105.82 : 0.41/0.59             |    2.621   |      Yes, p =  0.0392      |     1      |[74]Agc>Ngc|[70]gcC>gcN|[4]gtG>gtA|[2]agC>agT,tCc>tAc|[1]aAc>aGc,Aac...|

|    660     |     1      |    4.647   |            0.98/2378.36 : 0.78/0.22             |    1.749   |      Yes, p =  0.0784      |     2      |[78]tTG>tNN|[75]tCA>tNN|[70]gcA>gcN|[64]ccC>ccN|[41]aTT>aNN|[33]Gca>...|

|    784     |     1      |    1.751   |            0.81/3450.14 : 0.95/0.05             |   13.248   |      Yes, p =  0.0196      |     1      |[79]tgC>tgN|[55]GAg>NNg|[6]atT>atN|[1]aCC>aAG,aCC>aTT,Tcc>Ccc,TcC>Gc...|

|    804     |     1      |    7.381   |             0.41/20.20 : 0.88/0.12              |    1.010   |      Yes, p =  0.0980      |     0      |[59]GAg>NNg|[15]GAa>NNa|[5]Ata>Gta|[3]ctT>ctC,ttG>ttA|[2]gaG>gaA,Gta...|

|    808     |     1      |    5.447   |            0.00/62454.01 : 0.74/0.26            |  147.024   |      Yes, p =  0.0196      |     33     |[82]aaA>aaN|[77]Agt>Ngt|[11]GtC>CtG|[10]aaC>aaN|[8]CtG>GtC|[4]caA>ca...|

|    809     |     1      |   19.338   |            0.47/1249.24 : 0.74/0.26             |  124.844   |      Yes, p =  0.0196      |     21     |[75]AAt>NNt|[71]acC>acN|[1]aaA>aaG,aaC>aaG,AcC>GcN,Gtc>Atc,GTc>NNc,a...|

|    870     |     1      |   15.324   |             1.07/59.28 : 1.00/0.00              |    1.012   |      Yes, p =  0.0588      |     1      |[3]atC>atT|[2]gcG>gcA,ttC>ttT|[1]atC>atA,atT>atC,tTT>tGG,caA>caG,gcA...|

|    900     |     1      |    4.200   |            0.93/1071.21 : 0.67/0.33             |   54.375   |      Yes, p =  0.0196      |     11     |[79]aTA>aNN|[5]GAt>CTt|[2]acC>acN,aTA>aCC,Att>Gtt,ctG>ctT,Ctt>Att|[1...|

|    901     |     1      |   10.455   |            0.00/1443.95 : 0.79/0.21             |   10.084   |      Yes, p =  0.0196      |     14     |[79]Aat>Nat|[6]aaC>aaT|[4]CTT>GCA|[3]AAc>NNc,aaT>aaC,Ctt>Att|[2]ttC>...|

|    909     |     1      |    6.225   |            1.24/5155.45 : 0.70/0.30             |   13.764   |      Yes, p =  0.0196      |     2      |[6]atC>atN|[4]gTG>gNN|[3]aTC>aNN|[2]Aat>Gat,gtG>gtC,TGG>GAA|[1]ctT>c...|

|    911     |     1      |    4.439   |            0.57/4599.16 : 0.99/0.01             |   19.548   |      Yes, p =  0.0196      |     1      |[73]AAa>NNa|[5]aaA>aaG|[3]caG>caA|[2]acA>acN|[1]aAa>aCa,aAa>aGa,atC>...|

|    913     |     1      |    3.996   |             0.35/41.36 : 0.61/0.39              |    2.853   |      Yes, p =  0.0784      |     3      |[81]ttG>ttN|[3]ttC>ttT,ttT>ttC|[2]Acg>Gcg,gtG>gtA|[1]ACg>NNg,Ctt>Att...|

|    923     |     1      |   13.566   |             0.37/58.64 : 0.96/0.04              |    1.012   |      Yes, p =  0.0980      |     1      |[78]ttC>ttN|[48]GAg>NNg|[42]cTC>cNN|[30]ctC>ctN|[23]GAa>NNa|[4]gaG>g...|

|    991     |     1      |    7.938   |            0.49/5272.29 : 0.83/0.17             |  249.457   |      Yes, p =  0.0196      |     26     |[10]CCA>GTG|[7]GTG>CCA|[4]CCa>GTa|[3]ccT>ccC,gaC>gaT|[2]GTa>CCa,gtG>...|

|    1002    |     1      |    1.693   |              0.15/9.06 : 0.86/0.14              |    5.805   |      Yes, p =  0.0392      |     0      |[66]aaA>aaN|[17]ccC>ccN|[7]AaA>NaN|[4]Agt>Ggt|[3]ctT>ctC|[2]Ctt>Att|...|

|    1019    |     1      |    3.007   |             1.53/58.82 : 0.16/0.84              |    3.341   |      Yes, p =  0.0784      |     1      |[78]GcC>NcN|[76]Gta>Nta|[72]gcC>gcN|[33]tcC>tcN|[32]CAc>NNc|[25]AAc>...|

|    1020    |     1      |    4.619   |             0.49/479.57 : 0.56/0.44             |    3.962   |      Yes, p =  0.0392      |     6      |[95]GAc>NNc|[68]GAg>NNg|[21]GAa>NNa|[7]AGg>NNg|[3]Aca>Gca|[2]aaA>aaG...|

|    1075    |     1      |    0.004   |             0.00/15.18 : 0.01/0.99              |    4.218   |      Yes, p =  0.0588      |     0      |       [44]AAt>NNt|[3]Gat>Aat,GAt>NNt|[1]aaA>aaT,AaA>CaT,Aat>Gat       |

|    1115    |     1      |    0.000   |              0.00/8.63 : 0.84/0.16              |    2.904   |      Yes, p =  0.0980      |     4      |                 [2]Gcc>Tcc|[1]Gcc>Acc,gCc>gTc,TAc>GCc                 |

|    1160    |     1      |    0.547   |             0.32/46.53 : 0.85/0.15              |    7.358   |      Yes, p =  0.0392      |     2      |        [79]AAt>NNt|[1]Aat>Gat,AAT>GTG,gAt>gGt,GAT>TGC,tgC>tgN         |

|    1163    |     1      |    3.399   |             0.55/48.42 : 0.63/0.37              |    2.403   |      Yes, p =  0.0784      |     1      |[81]Ttt>Ntt|[58]ttC>ttN|[2]Cta>Tta,tGg>tTg|[1]ccT>ccC,Cta>Ata,ctA>ct...|

|    1176    |     1      |    4.165   |             1.36/22.93 : 0.44/0.56              |    1.372   |      Yes, p =  0.0980      |     1      |[50]GAa>NNa|[7]GAg>NNg|[2]Cgg>Agg,cgG>cgA,Gag>Nag,gTt>gCt,TGG>GTT|[1...|

|    1181    |     1      |    1.790   |             0.33/15.84 : 0.39/0.61              |    2.541   |      Yes, p =  0.0980      |     1      |[2]TtC>AtG,tTC>tCA|[1]Aca>Gca,CTT>ACN,CtT>TtC,Tca>Aca,TTc>NNc,tTC>tN...|

|    1185    |     1      |    4.397   |             0.58/46.28 : 0.92/0.08              |    0.950   |      Yes, p =  0.0392      |     1      |[73]ccA>ccN|[2]aTG>aNN,gcC>gcA|[1]aTG>aGC,atG>atT,gcA>gcT,gcC>gcT,AT...|

|    1191    |     1      |    1.938   |             0.35/78.81 : 0.61/0.39              |    3.002   |      Yes, p =  0.0588      |     2      |[78]atC>atN|[74]atA>atN|[2]aaT>aaC|[1]aAt>aGt,aTA>aAT,atA>atC,ATA>GC...|

|    1195    |     1      |    0.640   |             0.28/21.75 : 0.01/0.99              |    5.410   |      Yes, p =  0.0392      |     0      |[77]atC>atN|[1]atA>atG,Ata>Gta,Atc>Ttc,AtC>TtT,Att>Gtt,ttC>ttT,aTC>a...|

### ** Found _43_ sites under episodic diversifying positive selection at p <= 0.1**

(paml_env) fred@192 Downloads % 

H3 gene

Last login: Thu Oct 30 02:35:22 on ttys003

(base) fred@192 Downloads % conda activate /opt/miniconda3/envs/paml_env cd ~/Downloads

ArgumentError: activate does not accept more than one argument:

['/opt/miniconda3/envs/paml_env', 'cd', '/Users/fred/Downloads']

(base) fred@192 Downloads % conda config --add channels conda-forge 

Warning: 'conda-forge' already in 'channels' list, moving to the top

(base) fred@192 Downloads % conda config --add channels bioconda

Warning: 'bioconda' already in 'channels' list, moving to the top

(base) fred@192 Downloads % conda config --set channel_priority strict 

(base) fred@192 Downloads % conda install hyphy

2 channel Terms of Service accepted

Channels:

 - bioconda

 - conda-forge

 - defaults

Platform: osx-arm64

Collecting package metadata (repodata.json): done

Solving environment: done

==> WARNING: A newer version of conda exists. <==

    current version: 25.7.0

    latest version: 25.9.1

Please update conda by running

    $ conda update -n base -c conda-forge conda

# All requested packages already installed.

(base) fred@192 Downloads % hyphy i-

Error:

Could not read batch file '/Users/fred/Downloads/i-'.

Path stack:

	/opt/anaconda3/share/hyphy/

	/Users/fred/Downloads/

Check errors.log for execution error details.

(base) fred@192 Downloads % hyphy -i

HYPHY 2.5.64(MP) for Darwin on arm64 ARM Neon SIMD zlib (v1.2.13)

***************** TYPES OF STANDARD ANALYSES *****************

	(1) Selection Analyses

	(2) Evolutionary Hypothesis Testing

	(3) Relative evolutionary rate inference

	(4) Coevolutionary analysis

	(5) Basic Analyses

	(6) Codon Selection Analyses

	(7) Compartmentalization

	(8) Data File Tools

	(9) Miscellaneous

	(10) Model Comparison

	(11) Molecular Clock

	(12) Phylogeny Reconstruction

	(13) Positive Selection

	(14) Recombination

	(15) Selection/Recombination

	(16) Relative Rate

	(17) Relative Ratio

 Please select type of analyses you want to list (or press ENTER to process custom batch file):1

***************** FILES IN 'Selection Analyses' ***************** 

	(1) [MEME] Test for episodic site-level selection using MEME (Mixed Effects Model of Evolution).

	(2) [FEL] Test for pervasive site-level selection using FEL (Fixed Effects Likelihood).

	(3) [SLAC] Test for pervasive site-level selection using SLAC (Single Likelihood Ancestor Counting).

	(4) [FUBAR] Test for pervasive site-level selection using FUBAR (Fast Unconstrained Bayesian AppRoximation for inferring selection).

	(5) [BUSTED] Test for episodic gene-wide selection using BUSTED (Branch-site Unrestricted Statistical Test of Episodic Diversification).

	(6) [aBSREL] Test for lineage-specific evolution using the branch-site method aBS-REL (Adaptive Branch-Site Random Effects Likelihood).

	(7) [RELAX] Test for relaxation of selection pressure along a specified set of test branches using RELAX (a random effects test of selection relaxation).

	(8) [FADE] Test a protein alignment for directional selection towards specific amino acids along a specified set of test branches using FADE (a FUBAR Approach to Directional Evolution).

	(9) [PRIME] 

	(10) [Error-Filter] Use a BUSTED-E model fit to clean-up a sequence alignment

 Please select the analysis you would like to perform (or press ENTER to return to the list of analysis types):1

Analysis Description

--------------------

MEME (Mixed Effects Model of Evolution) estimates a site-wise synonymous

(&alpha;) and a two-category mixture of non-synonymous (&beta;-, with

proportion p-, and &beta;+ with proportion [1-p-]) rates, and uses a

likelihood ratio test to determine if &beta;+ > &alpha; at a site. The

estimates aggregate information over a proportion of branches at a site,

so the signal is derived from episodic diversification, which is a

combination of strength of selection [effect size] and the proportion of

the tree affected. A subset of branches can be selected for testing as

well, in which case an additional (nuisance) parameter will be inferred

-- the non-synonymous rate on branches NOT selected for testing.

Multiple partitions within a NEXUS file are also supported for

recombination - aware analysis. Version 3.0 adds a different format for

ancestral state reconstruction, branch-site posterior storage, and

site-level heterogeneity testing. Version 4 adds support for multiple

hits and more than 2 rate classes on omega, as well as site-level

imputation option 

- __Requirements__: in-frame codon alignment and a phylogenetic tree

- __Citation__: Detecting Individual Sites Subject to Episodic Diversifying Selection.

_PLoS Genet_ 8(7): e1002764.

- __Written by__: Sergei L. Kosakovsky Pond, Steven Weaver

- __Contact Information__: spond@temple.edu

- __Analysis Version__: 4.0

####Choose Genetic Code

1. [**Universal**] Universal code. (Genebank transl_table=1).

2. [**Vertebrate-mtDNA**] Vertebrate mitochondrial DNA code. (Genebank transl_table=2).

3. [**Yeast-mtDNA**] Yeast mitochondrial DNA code. (Genebank transl_table=3).

4. [**Mold-Protozoan-mtDNA**] Mold, Protozoan and Coelenterate mitochondrial DNA and the Mycloplasma/Spiroplasma code. (Genebank transl_table=4).

5. [**Invertebrate-mtDNA**] Invertebrate mitochondrial DNA code. (Genebank transl_table=5).

6. [**Ciliate-Nuclear**] Ciliate, Dasycladacean and Hexamita Nuclear code. (Genebank transl_table=6).

7. [**Echinoderm-mtDNA**] Echinoderm mitochondrial DNA code. (Genebank transl_table=9).

8. [**Euplotid-Nuclear**] Euplotid Nuclear code. (Genebank transl_table=10).

9. [**Alt-Yeast-Nuclear**] Alternative Yeast Nuclear code. (Genebank transl_table=12).

10. [**Ascidian-mtDNA**] Ascidian mitochondrial DNA code. (Genebank transl_table=13).

11. [**Flatworm-mtDNA**] Flatworm mitochondrial DNA code. (Genebank transl_table=14).

12. [**Blepharisma-Nuclear**] Blepharisma Nuclear code. (Genebank transl_table=15).

13. [**Chlorophycean-mtDNA**] Chlorophycean Mitochondrial Code (transl_table=16).

14. [**Trematode-mtDNA**] Trematode Mitochondrial Code (transl_table=21).

15. [**Scenedesmus-obliquus-mtDNA**] Scenedesmus obliquus mitochondrial Code (transl_table=22).

16. [**Thraustochytrium-mtDNA**] Thraustochytrium Mitochondrial Code (transl_table=23).

17. [**Pterobranchia-mtDNA**] Pterobranchia Mitochondrial Code (transl_table=24).

18. [**SR1-and-Gracilibacteria**] Candidate Division SR1 and Gracilibacteria Code (transl_table=25).

19. [**Pachysolen-Nuclear**] Pachysolen tannophilus Nuclear Code (transl_table=26).

20. [**Mesodinium-Nuclear**] Mesodinium Nuclear Code (transl_table=29)

21. [**Peritrich-Nuclear**] Peritrich Nuclear Code (transl_table=30)

22. [**Cephalodiscidae-mtDNA**] Cephalodiscidae Mitochondrial UAA-Tyr Code (transl_table=33)

>Please choose an option (or press q to cancel selection):1

>Select a coding sequence alignment file (`/Users/fred/Downloads/`) H3_master_TRIMMED.fas  

-------

>[WARNING] '/Users/fred/Downloads/H3_master_TRIMMED.fas' contains 1

duplicate sequence. Identical sequences do not contribute any

information to the analysis and only slow down computation. Please

consider removing duplicate or 'nearly' duplicate sequences, e.g. using

https://github.com/veg/hyphy-analyses/tree/master/remove-duplicates

prior to running selection analyses

-------

>Please select a tree file for the data: (`/Users/fred/Downloads/`) H3_FINAL.tree

/Users/fred/Downloads/H3_FINAL.tree

H3_FINAL.tree

>Loaded a multiple sequence alignment with **620** sequences, **1238** codons, and **1** partitions from `/Users/fred/Downloads/H3_master_TRIMMED.fas`

####Choose the set of branches to test for selection

1. [**All**] Include all branches in the analysis

2. [**Internal**] Include all internal branches in the analysis

3. [**Leaves**] Include all leaf branches in the analysis

4. [**Unlabeled branches**] Set of 1237 unlabeled branches

>Please choose an option (or press q to cancel selection):1

>Select the p-value threshold to use when testing for selection (permissible range = [0,1], default value = 0.1): 0.1

>[Advanced setting, will result in MUCH SLOWER run time] Perform parametric bootstrap resampling to derive site-level null LRT distributions up to this many replicates per site. Recommended use for small to medium (<30 sequences) datasets (permissible range = [0,1000], default value = 50, integer): 50

The number omega rate classes to include in the model [2 is the strongly recommended default] (permissible range = [2,4], default value = 2, integer): 2

####Include support for multiple nucleotide substitutions

1. [**Double**] Include branch-specific rates for double nucleotide substitutions

2. [**Double+Triple**] Include branch-specific rates for double and triple nucleotide substitutions

3. [**None**] [Default] Use standard models which permit only single nucleotide changes to occur instantly

>Please choose an option (or press q to cancel selection):3

####Impute likely states for sequences

1. [**Yes**] Impute marginal likelihoods for each codon at each sequence and each site

2. [**No**] Do not impute marginal likelihoods for each codon at each sequence and each site

>Please choose an option (or press q to cancel selection):2

####Optimization precision settings for preliminary fits

1. [**standard**] [Default] Use standard optimization settings.

2. [**reduced**] Cruder optimizations settings for faster fitting of preliminary models

>Please choose an option (or press q to cancel selection):1

>Save the resulting JSON file to (`/Users/fred/Downloads/`) MEME_H3_results.json

### Branches to include in the MEME analysis

Selected 1237 branches to include in the MEME analysis: `seq448, seq366, seq414, seq27, seq391, Node8, Node6, seq96, seq430, Node11, Node5, Node3, Node1, seq514, seq420, seq213, seq266, Node22, Node20, seq271, seq402, seq443, Node28, Node26, seq293, Node25, Node19, seq55, seq579, Node34, seq455, seq194, seq107, seq219, Node42, Node40, Node38, seq305, seq582, Node45, Node37, Node33, seq355, seq508, Node50, seq502, seq104, seq159, Node55, Node53, Node49, seq115, seq178, seq287, Node64, Node62, seq491, seq585, Node67, Node61, seq174, seq316, seq441, Node79, seq286, seq202, seq372, Node91, seq396, seq490, seq125, Node100, seq77, seq413, Node105, seq390, seq187, Node108, Node104, seq608, seq207, seq578, Node114, Node112, seq384, seq453, Node117, Node111, Node103, Node99, Node97, seq601, seq20, Node120, Node96, seq30, Node95, seq57, seq614, Node124, Node94, Node90, seq418, Node89, seq435, seq49, seq169, Node131, Node129, seq298, Node128, Node88, Node86, seq101, Node85, seq276, seq303, seq429, Node139, seq67, seq83, Node142, Node138, Node136, Node84, seq88, seq292, seq119, seq181, Node152, Node150, seq496, seq594, Node155, Node149, Node147, seq108, seq163, Node159, seq513, seq43, seq212, seq70, Node168, Node166, Node164, seq505, Node163, seq37, seq95, Node172, Node162, Node158, Node146, seq379, seq528, seq136, seq25, Node179, Node177, Node175, Node145, Node83, seq360, seq367, seq157, seq133, seq472, Node190, Node188, Node186, Node184, seq519, seq586, seq113, seq460, Node199, Node197, seq222, seq310, Node203, seq61, seq191, Node206, Node202, Node196, Node194, seq407, seq447, Node210, seq218, seq425, Node213, Node209, Node193, Node183, seq270, seq15, seq466, Node218, Node216, Node182, Node82, Node78, Node76, seq199, seq267, seq171, seq438, Node231, seq463, seq32, seq204, Node239, seq93, Node238, seq313, Node237, Node235, seq363, seq126, seq155, seq469, Node249, Node247, Node245, seq86, seq492, seq589, seq177, seq117, seq289, Node261, Node259, Node257, Node255, Node253, seq487, seq64, seq17, Node274, Node272, seq449, Node271, seq97, seq416, seq28, seq393, Node285, Node283, seq432, Node282, Node280, seq369, Node279, seq382, seq522, Node290, Node278, Node270, seq301, seq454, Node293, Node269, seq58, seq581, Node297, seq220, seq112, seq196, Node303, Node301, seq457, seq306, seq596, Node308, Node306, Node300, Node296, Node268, seq273, seq404, seq444, Node316, Node314, seq422, seq11, seq21, seq279, Node323, Node321, Node319, Node313, seq295, Node312, seq375, seq80, seq410, seq73, seq605, Node336, Node334, Node332, seq283, Node331, Node329, seq51, Node328, seq121, seq185, seq602, Node343, Node341, Node327, Node311, Node267, seq516, Node266, seq46, seq166, Node349, seq387, seq399, Node352, Node348, seq507, seq102, seq161, Node358, seq510, seq357, seq501, seq617, Node366, seq190, seq40, seq210, Node372, Node370, seq69, seq498, Node375, Node369, Node365, Node363, Node361, Node357, Node355, Node347, Node265, seq215, seq479, seq611, seq134, seq529, Node384, Node382, Node380, Node378, Node264, Node252, Node244, Node234, Node230, Node228, seq575, Node227, Node225, seq484, Node224, seq480, Node223, seq483, seq349, seq570, seq474, seq264, seq6, seq332, seq538, Node411, Node409, seq238, seq330, Node415, seq254, seq242, seq145, Node421, Node419, seq328, Node418, Node414, Node408, Node406, Node404, seq7, seq234, seq248, seq540, Node431, Node429, seq151, seq232, Node435, seq230, seq592, Node438, Node434, Node428, seq139, seq597, seq326, seq568, Node449, Node447, seq240, seq476, Node454, seq246, seq550, Node457, Node453, seq546, Node452, Node446, seq340, seq260, seq236, Node464, Node462, seq262, seq318, Node468, seq536, Node467, Node461, Node445, seq336, seq324, seq5, seq141, seq255, seq346, seq554, Node485, seq322, seq562, Node488, Node484, Node482, Node480, Node478, Node476, Node474, seq320, seq258, seq227, seq147, Node495, Node493, Node491, Node473, seq552, Node472, Node444, seq149, seq250, seq348, seq143, seq556, Node505, Node503, Node501, Node499, Node443, Node441, Node427, Node425, Node403, seq534, seq544, seq338, seq566, Node513, Node511, Node509, seq532, seq341, seq344, seq252, seq547, seq564, seq244, seq352, Node528, Node526, Node524, Node522, Node520, Node518, Node516, Node508, Node402, Node400, seq572, seq334, seq354, Node533, Node531, Node399, seq542, Node398, seq560, Node397, seq558, Node396, Node394, seq571, seq333, seq353, Node543, Node541, seq263, seq335, Node553, seq345, seq553, Node560, seq561, seq321, Node563, Node559, seq256, Node558, seq4, Node557, seq323, seq140, Node568, Node556, Node552, seq257, seq319, seq146, seq228, Node576, Node574, Node572, seq233, seq595, seq325, seq567, Node586, Node584, seq261, seq317, Node589, Node583, Node581, seq235, seq545, seq239, seq475, Node601, seq245, seq549, Node604, Node600, Node598, seq551, Node597, seq259, Node596, seq249, seq347, seq142, seq555, Node614, Node612, seq148, Node611, Node609, Node595, seq339, Node594, Node592, Node580, seq535, Node579, Node571, Node551, seq533, seq543, seq337, seq565, Node625, Node623, Node621, seq8, Node620, Node550, seq138, Node549, seq569, Node548, seq559, Node547, seq541, Node546, Node540, seq343, seq251, seq548, seq243, seq351, seq563, Node642, Node640, Node638, Node636, Node634, seq342, seq223, seq473, Node648, Node646, seq531, seq224, seq226, seq225, Node656, Node654, Node652, seq144, seq253, seq241, Node663, seq331, seq537, Node667, seq327, seq237, seq329, Node672, Node670, Node666, Node662, Node660, seq247, seq539, Node676, seq150, seq231, seq350, Node682, Node680, seq590, seq229, seq557, Node687, Node685, Node679, Node675, Node659, Node651, Node645, Node633, Node539, Node393, Node391, seq315, seq94, seq365, seq471, seq129, seq154, Node701, Node699, Node697, Node695, seq376, seq489, seq619, seq42, seq192, seq71, Node721, Node719, Node717, seq82, Node716, seq66, Node715, Node713, Node711, seq406, seq446, Node726, Node710, seq518, seq304, seq275, seq309, seq383, seq524, Node744, seq297, Node743, Node741, seq123, seq100, seq31, seq394, Node753, Node751, seq434, seq3, Node758, seq412, Node757, seq209, Node756, Node750, Node748, Node740, seq75, seq606, Node764, seq452, Node763, Node739, seq285, seq419, Node768, Node738, seq18, seq280, Node771, Node737, seq13, seq54, Node774, Node736, Node734, seq371, Node733, Node731, Node729, Node709, seq459, seq584, Node780, seq111, seq221, Node783, Node779, seq59, Node778, Node708, seq2, seq1, Node787, Node707, seq359, seq47, seq168, Node793, seq389, seq401, Node796, Node792, Node790, Node706, seq89, seq291, seq118, seq179, Node804, seq495, seq593, Node807, Node803, Node801, Node799, Node705, seq175, seq440, Node812, seq465, seq506, Node815, Node811, seq268, Node810, Node704, Node694, seq35, seq512, seq105, seq162, Node825, Node823, Node821, seq216, seq424, Node829, seq613, seq137, seq530, Node834, Node832, Node828, Node820, seq201, seq577, Node837, Node819, Node693, Node691, seq493, seq85, seq478, seq203, seq462, seq33, seq311, Node853, Node851, Node849, Node847, seq172, seq437, Node857, seq265, seq214, seq131, seq526, Node864, Node862, Node860, Node856, Node846, seq91, seq574, seq56, seq580, Node875, seq456, seq307, seq583, Node881, Node879, seq109, seq193, Node884, Node878, Node874, seq486, seq409, seq74, seq604, Node894, Node892, Node890, seq23, seq277, Node898, seq610, Node897, Node889, seq374, seq197, seq450, Node906, Node904, seq52, seq385, seq398, Node914, seq45, seq165, Node917, Node913, seq294, seq380, seq520, Node922, Node920, Node912, seq368, seq184, seq599, Node928, seq26, seq392, Node934, seq282, seq415, Node937, Node933, seq98, Node932, seq431, Node931, Node927, Node925, Node911, Node909, Node903, seq300, seq427, Node943, seq62, seq616, seq182, seq39, seq211, seq500, Node956, Node954, Node952, Node950, Node948, seq78, Node947, seq16, Node946, Node942, Node902, Node888, seq515, seq421, seq10, seq122, Node966, seq272, seq403, seq442, Node972, Node970, seq152, Node969, Node965, Node963, Node961, Node887, Node873, seq356, seq503, seq509, seq103, seq158, Node982, Node980, Node978, Node976, Node872, Node870, seq362, seq128, seq468, Node987, Node985, Node869, Node867, Node845, Node843, Node841, seq587, seq176, seq114, seq288, Node994, Node992, Node990, Node840, Node690, Node390, Node222, seq290, seq116, seq180, Node1003, Node1001, seq87, seq494, seq591, Node1008, Node1006, Node1000, seq173, seq439, Node1013, seq314, seq517, Node1017, seq504, seq405, seq445, Node1024, seq458, seq110, seq195, Node1030, Node1028, seq308, seq588, Node1033, Node1027, Node1023, Node1021, seq364, seq470, seq130, seq156, Node1041, Node1039, Node1037, seq411, seq76, seq607, Node1049, Node1047, seq423, seq217, Node1052, Node1046, seq377, seq612, seq135, seq527, Node1059, Node1057, Node1055, Node1045, seq481, seq106, seq160, Node1064, Node1062, Node1044, Node1036, Node1020, Node1016, Node1012, seq65, seq274, Node1070, seq302, seq428, Node1073, Node1069, seq12, seq600, seq186, Node1083, Node1081, seq370, Node1080, seq29, seq395, Node1090, seq284, seq417, Node1093, Node1089, seq99, Node1088, seq433, Node1087, Node1079, seq48, seq167, Node1100, seq388, seq400, Node1103, Node1099, seq60, seq381, seq523, Node1108, Node1106, Node1098, Node1078, seq200, seq488, seq189, seq41, seq618, Node1118, Node1116, Node1114, Node1112, seq19, seq451, Node1121, Node1111, Node1077, seq206, seq24, Node1126, seq124, Node1125, seq53, seq81, Node1130, Node1124, Node1076, Node1068, seq358, seq511, Node1134, seq296, seq36, seq92, Node1139, Node1137, Node1133, Node1067, Node1011, Node999, seq269, seq576, Node1142, Node998, seq464, Node997, Node221, Node75, seq482, Node74, seq461, Node73, seq312, Node72, seq436, seq198, seq573, Node1152, Node1150, seq170, Node1149, Node71, seq34, seq620, Node1158, seq90, Node1157, seq361, seq127, seq153, Node1165, seq84, seq467, Node1168, Node1164, Node1162, Node1156, Node70, Node60, seq477, seq525, seq132, seq609, Node1175, Node1173, Node1171, Node59, seq408, seq72, seq79, seq603, Node1184, Node1182, Node1180, seq63, seq485, Node1188, seq281, seq22, seq278, Node1195, Node1193, seq188, seq497, seq615, seq499, Node1203, Node1201, Node1199, seq68, seq38, seq208, Node1208, Node1206, Node1198, Node1192, seq373, Node1191, Node1187, Node1179, seq205, seq50, seq183, seq598, Node1217, seq9, seq120, Node1220, Node1216, Node1214, Node1212, Node1178, Node58, Node48, Node32, Node18, Node16, seq14, seq299, seq426, Node1225, Node1223, Node15, seq378, seq521, Node1228, Node14, seq44, seq164, Node1232, seq386, seq397, Node1235, Node1231`

### Obtaining branch lengths and nucleotide substitution biases under the nucleotide GTR model

>Use/Save parameter estimates from 'initial-guess' model fits (`/Users/fred/Downloads/`) null

####Reduce zero-length branches

1. [**Yes**] Automatically delete internal zero-length branches for computational efficiency (will not affect results otherwise)

2. [**Constrain**] Keep zero-length branches, but constrain their values to 0

3. [**No**] Keep all branches

>Please choose an option (or press q to cancel selection):1

### Deleted 106 zero-length internal branches: `Node1, Node1003, Node103, Node1041, Node108, Node1080, Node1083, Node1088, Node1112, Node1118, Node112, Node1121, Node1124, Node1125, Node1130, Node1182, Node1191, Node1201, Node1203, Node1206, Node1208, Node128, Node145, Node152, Node155, Node162, Node163, Node168, Node179, Node194, Node199, Node202, Node206, Node237, Node238, Node239, Node270, Node274, Node278, Node282, Node303, Node361, Node370, Node375, Node414, Node418, Node434, Node444, Node446, Node462, Node467, Node472, Node473, Node480, Node484, Node488, Node501, Node556, Node558, Node563, Node581, Node583, Node592, Node594, Node595, Node596, Node611, Node64, Node642, Node679, Node709, Node715, Node716, Node721, Node729, Node734, Node737, Node738, Node739, Node740, Node748, Node750, Node756, Node757, Node763, Node771, Node804, Node810, Node853, Node887, Node89, Node90, Node912, Node932, Node933, Node94, Node947, Node95, Node952, Node954, Node956, Node96, Node969, Node97, Node99, Node998`

* Log(L) = -78293.82, AIC-c = 159078.99 (1245 estimated parameters)

* 1 partition. Total tree length by partition (subs/site) 43.867

### Obtaining the global omega estimate based on relative GTR branch lengths and nucleotide substitution biases

* Log(L) = -74528.70, AIC-c = 151352.82 (1146 estimated parameters)

* 1 partition. Total tree length by partition (subs/site) 50.061

* non-synonymous/synonymous rate ratio for *test* =   0.2033

####Perform branch length re-optimization under the full codon model

1. [**Yes**] [Default] Perform branch length re-optimization under the full codon model

2. [**No**] Skip branch length re-optimization under the full codon model (faster but less precise)

>Please choose an option (or press q to cancel selection):1

Only analyze sites whose 1-based indices match the following list (null to skip) : null

For sites whose 1-based indices match the following list, write out likelihood function snapshots (null string to skip) : null string

### Improving branch lengths, nucleotide substitution biases, and global dN/dS ratios under a full codon model

* Log(L) = -74105.61

* Log(L) = -74105.61, AIC-c = 150506.65 (1146 estimated parameters)

* 1 partition. Total tree length by partition (subs/site) 74.079

* non-synonymous/synonymous rate ratio for *test* =   0.1452

### For partition 1 these sites are significant at p <=0.1

|   Codon    | Partition  |   alpha    |non-syn rate (beta) distribution, rates : weights|    LRT     |Episodic selection detected?| # branches |         List of most common codon substitutions at this site          |

|:----------:|:----------:|:----------:|:-----------------------------------------------:|:----------:|:--------------------------:|:----------:|:---------------------------------------------------------------------:|

|     34     |     1      |    6.921   |            0.89/19494.89 : 0.83/0.17            |   11.703   |      Yes, p =  0.0196      |     1      |[67]Agc>Ngc|[51]CAa>NNa|[33]CAg>NNg|[7]AGc>NNc|[3]aaT>aaC,Agt>Ngt|[2...|

|     35     |     1      |    9.553   |             1.00/809.17 : 0.86/0.14             |    8.808   |      Yes, p =  0.0196      |     6      |[4]aCt>aTt|[2]acC>acT,aCC>aTT,acT>acC,aTG>aCT,caA>caG|[1]aaG>aaA,aCt...|

|     42     |     1      |    3.947   |             0.73/288.41 : 0.84/0.16             |    3.236   |      Yes, p =  0.0588      |     6      |[66]Aca>Nca|[11]Gac>Nac|[9]Aac>Nac|[7]Acg>Ncg|[3]aGc>aAc,AGc>NAc|[2]...|

|    183     |     1      |    6.093   |             0.00/52.12 : 0.85/0.15              |    1.658   |      Yes, p =  0.0980      |     1      |                          [1]GAc>AGc,gaC>gaT                           |

|    209     |     1      |   23.558   |             0.00/765.96 : 0.74/0.26             |    3.248   |      Yes, p =  0.0392      |     0      |[55]TTc>NNc|[3]CTc>NNc,TTC>NNT|[2]ttC>ttT,TTt>NNt,ttT>ttC|[1]TTc>AGc...|

|    232     |     1      |    3.235   |             0.82/16.71 : 0.57/0.43              |    1.452   |      Yes, p =  0.0588      |     1      |[74]AAt>NNt|[16]taC>taN|[2]gaG>gaA,tAC>tCT|[1]Aag>Gag,AAT>NNC,aGg>aA...|

|    243     |     1      |    8.518   |             0.45/26.44 : 0.53/0.47              |    1.852   |      Yes, p =  0.0980      |     2      |[148]Gaa>Naa|[76]Caa>Naa|[65]ggC>ggN|[6]Gag>Nag|[5]Cag>Nag|[4]GgC>Ng...|

|    283     |     1      |    4.166   |             0.64/67.85 : 1.00/0.00              |    2.122   |      Yes, p =  0.0392      |     1      |[70]AGa>NNa|[57]AAc>NNc|[10]Gaa>Naa|[4]AAa>NNa|[2]acC>acA,acC>acN|[1...|

|    307     |     1      |    0.000   |             0.00/35.68 : 0.73/0.27              |    3.262   |      Yes, p =  0.0588      |     1      |                              [1]GTT>CGA                               |

|    323     |     1      |    6.304   |             0.55/25.24 : 0.98/0.02              |    1.393   |      Yes, p =  0.0588      |     1      |[75]GAt>NNt|[47]GAg>NNg|[33]GAa>NNa|[4]caG>caA|[3]Gag>Nag|[2]ctA>ctG...|

|    356     |     1      |    0.898   |             0.57/46.21 : 0.34/0.66              |    8.897   |      Yes, p =  0.0196      |     1      |[77]atC>atN|[64]AcA>NcN|[61]aTT>aNN|[20]ccC>ccN|[11]ctC>ctN|[6]Aca>N...|

|    359     |     1      |    2.913   |             0.22/45.02 : 0.69/0.31              |   10.093   |      Yes, p =  0.0196      |     11     |[82]tTA>tNN|[79]aTA>aNN|[17]aTC>aNN|[5]aGa>aAa|[4]gTa>gCa|[2]atC>atT...|

|    368     |     1      |    4.432   |             0.79/26.84 : 0.88/0.12              |    1.065   |      Yes, p =  0.0980      |     0      |[76]Aca>Nca|[75]ATt>NNt|[73]aTG>aNN|[10]AGg>NNg|[4]gaA>gaG|[3]aTG>aC...|

|    373     |     1      |   12.148   |             1.06/106.36 : 0.82/0.18             |    1.375   |      Yes, p =  0.0392      |     1      |[5]agT>agC|[3]agA>agG,ggA>ggG,ggG>ggA|[2]AAa>GGa,aTG>aCA,Gga>Aga|[1]...|

|    445     |     1      |    5.100   |             2.57/93.87 : 0.87/0.13              |    2.636   |      Yes, p =  0.0588      |     1      |[78]Gtt>Ntt|[70]cAC>cNN|[39]tGG>tNN|[33]cGG>cNN|[5]tAC>tNN|[4]aAc>aG...|

|    446     |     1      |    5.475   |             0.36/111.65 : 0.68/0.32             |    5.713   |      Yes, p =  0.0196      |     4      |[79]gTC>gNN|[78]tCG>tNN|[75]Ttg>Ntg|[73]cTC>cNN|[3]atC>atT|[2]cCG>cN...|

|    474     |     1      |    5.280   |             0.69/91.48 : 1.00/0.00              |    3.621   |      Yes, p =  0.0588      |     2      |[75]gTA>gNN|[65]aTG>aNN|[3]aAA>aNN|[2]aaA>aaG,aTG>aAA,tcT>tcC,tCt>tT...|

|    476     |     1      |    6.756   |             0.68/32.60 : 1.00/0.00              |    1.816   |      Yes, p =  0.0784      |     1      |[20]aTG>aNN|[4]cgG>cgA|[3]Aga>Gga|[2]agA>agG,ggA>ggG,TgG>GgA|[1]aGa>...|

|    571     |     1      |    7.299   |             1.40/96.34 : 0.90/0.10              |    2.538   |      Yes, p =  0.0588      |     1      |[74]Agc>Ngc|[70]gcC>gcN|[4]gtG>gtA|[2]agC>agT,tCc>tAc|[1]aAc>aGc,Aac...|

|    660     |     1      |    4.630   |            0.89/1635.13 : 1.00/0.00             |    2.055   |      Yes, p =  0.0588      |     3      |[78]tTG>tNN|[75]tCA>tNN|[70]gcA>gcN|[64]ccC>ccN|[41]aTT>aNN|[33]Gca>...|

|    784     |     1      |    1.289   |             0.65/527.82 : 0.61/0.39             |   12.464   |      Yes, p =  0.0196      |     2      |[79]tgC>tgN|[55]GAg>NNg|[6]atT>atN|[1]aCC>aAG,aCC>aTT,Acc>Tcc,ACC>TG...|

|    787     |     1      |    7.309   |            1.21/14165.36 : 0.77/0.23            |    6.629   |      Yes, p =  0.0196      |     2      |[78]Tca>Nca|[76]Tgc>Ngc|[71]gtA>gtN|[43]Ctt>Ntt|[5]Tcc>Ncc|[4]AAa>NN...|

|    808     |     1      |    7.209   |            0.68/68822.27 : 0.71/0.29            |  187.360   |      Yes, p =  0.0196      |     24     |[82]aaA>aaN|[77]Cgt>Ngt|[11]GtC>CtG|[10]aaC>aaN|[8]CtG>GtC|[4]caA>ca...|

|    809     |     1      |   19.304   |            0.46/1254.10 : 0.74/0.26             |  124.844   |      Yes, p =  0.0196      |     21     |[75]AAt>NNt|[71]acC>acN|[14]AAc>GTc|[10]GAc>NNc|[9]AAc>NNc|[8]aaG>aa...|

|    827     |     1      |   11.988   |             0.57/21.78 : 0.84/0.16              |    0.387   |      Yes, p =  0.0784      |     2      |[17]Gag>Nag|[8]Gaa>Naa|[7]gaG>gaA|[4]AGg>NNg,gaA>gaG|[2]AaA>CaT,agA>...|

|    900     |     1      |    4.355   |            0.90/1064.88 : 0.48/0.52             |   54.391   |      Yes, p =  0.0196      |     11     |[79]aTA>aNN|[5]GAt>CTt|[2]acC>acN,aTA>aCC,Att>Gtt,ctG>ctT,Ctt>Att|[1...|

|    901     |     1      |   20.079   |            0.80/9652.09 : 0.75/0.25             |   51.115   |      Yes, p =  0.0196      |     6      |[79]Tat>Nat|[5]CTT>GCA|[4]aaC>aaT|[3]AAc>NNc,aaT>aaC,Ctt>Att|[2]TtC>...|

|    905     |     1      |   12.290   |             1.13/38.94 : 0.73/0.27              |    0.527   |      Yes, p =  0.0784      |     1      |[73]TGg>NNg|[68]Agg>Ngg|[13]Aga>Nga|[4]aTG>aNN|[3]agG>agA,ttC>ttT|[2...|

|    909     |     1      |    6.081   |            0.57/3026.37 : 0.78/0.22             |   10.032   |      Yes, p =  0.0196      |     3      |[6]atC>atN|[4]gTG>gNN|[3]aTC>aNN|[2]Aat>Gat,gtG>gtC|[1]ctT>ctC,Gaa>A...|

|    911     |     1      |    5.057   |            0.71/5187.46 : 0.91/0.09             |   19.637   |      Yes, p =  0.0196      |     1      |[73]AAa>NNa|[5]aaA>aaG|[3]caG>caA|[2]acA>acN|[1]aAa>aCa,aAa>aGa,aAA>...|

|    913     |     1      |    4.039   |             0.35/42.97 : 0.44/0.56              |    2.858   |      Yes, p =  0.0980      |     3      |[81]ttG>ttN|[3]ttC>ttT,ttT>ttC|[2]Acg>Gcg,gtG>gtA|[1]ACg>NNg,Ctt>Att...|

|    917     |     1      |    5.057   |             0.84/27.09 : 0.39/0.61              |    2.449   |      Yes, p =  0.0980      |     1      |[69]GAg>NNg|[56]CAa>NNa|[46]Gaa>Naa|[19]AAa>NNa|[15]CAg>NNg|[4]GAa>N...|

|    921     |     1      |    8.670   |             2.19/406.55 : 0.43/0.57             |    6.493   |      Yes, p =  0.0196      |     2      |[71]CAg>NNg|[67]GcC>NcN|[9]CAa>NNa|[6]gcC>gcN|[5]caG>caA|[4]Gcc>Ncc|...|

|    923     |     1      |   13.106   |             0.37/51.71 : 0.77/0.23              |    0.982   |      Yes, p =  0.0980      |     1      |[78]ttC>ttN|[48]GAg>NNg|[42]cTC>cNN|[30]ctC>ctN|[23]GAa>NNa|[4]gaG>g...|

|    930     |     1      |    2.263   |             0.55/81.76 : 1.00/0.00              |    4.097   |      Yes, p =  0.0196      |     1      |[31]acC>acN|[19]acA>acN|[1]aAc>aCc,aAc>aGc,Aac>Gac,AAC>TTT,acC>acA,G...|

|    937     |     1      |    9.337   |             0.97/55.51 : 1.00/0.00              |    1.393   |      Yes, p =  0.0392      |     1      |[85]GAa>NNa|[4]taC>taN,tcC>tcT|[2]TGG>GAA|[1]gaA>gaG,gAa>gGa,TCC>NGA...|

|    945     |     1      |    3.183   |             0.50/27.47 : 0.52/0.48              |    1.824   |      Yes, p =  0.0980      |     0      |[70]gTT>gNN|[2]aTT>aNN,Ctg>Atg,Ctg>Ttg,Gtt>Att|[1]Atg>Ctg,AtG>GtT,AT...|

|    950     |     1      |    0.563   |              0.00/8.41 : 0.57/0.43              |    3.152   |      Yes, p =  0.0784      |     2      |     [2]aaC>aaN,aTA>aNN|[1]aaC>aaT,aAC>aCA,aTA>aAC,ATa>CCa,Ata>Gta     |

|    991     |     1      |    7.938   |            0.49/5339.97 : 0.75/0.25             |  249.464   |      Yes, p =  0.0196      |     26     |[10]CCA>GTG|[7]GTG>CCA|[4]CCa>GTa|[3]ccT>ccC,gaC>gaT|[2]GTa>CCa,gtG>...|

|    996     |     1      |    5.707   |             0.66/31.87 : 0.96/0.04              |    0.499   |      Yes, p =  0.0980      |     0      |[71]aaA>aaN|[70]Aac>Nac|[69]Aag>Nag|[29]AAc>NNc|[10]AAt>NNt|[7]Agg>N...|

|    1019    |     1      |    3.125   |             1.34/65.48 : 0.99/0.01              |    3.463   |      Yes, p =  0.0392      |     1      |[78]GcC>NcN|[76]Gta>Nta|[72]gcC>gcN|[33]tcC>tcN|[32]CAc>NNc|[25]AAc>...|

|    1020    |     1      |    5.125   |             0.43/466.88 : 1.00/0.00             |    3.827   |      Yes, p =  0.0196      |     6      |[95]GAc>NNc|[68]GAg>NNg|[21]GAa>NNa|[7]AGg>NNg|[3]Aca>Gca|[2]aaA>aaG...|

|    1128    |     1      |    9.407   |            0.00/3876.26 : 0.83/0.17             |    3.125   |      Yes, p =  0.0392      |     1      |                 [6]Gca>Nca|[1]gcA>gcG,gcA>gcT,gCa>gGa                 |

|    1160    |     1      |    0.365   |             0.36/44.63 : 0.17/0.83              |    7.483   |      Yes, p =  0.0392      |     1      |        [79]AAt>NNt|[1]Aat>Gat,AAT>GTG,gAt>gGt,GAT>TGC,tgC>tgN         |

|    1163    |     1      |    3.469   |             0.55/50.04 : 0.40/0.60              |    2.407   |      Yes, p =  0.0588      |     1      |[81]Ttt>Ntt|[58]ttC>ttN|[2]Cta>Tta,tGg>tTg|[1]ccT>ccC,Cta>Ata,ctA>ct...|

|    1181    |     1      |    1.791   |             0.33/15.90 : 0.56/0.44              |    2.545   |      Yes, p =  0.0784      |     1      |[2]TtC>AtG,tTC>tCA|[1]Aca>Gca,CTT>ACN,CtT>TtC,Tca>Aca,TTc>NNc,tTC>tN...|

|    1185    |     1      |    4.546   |             0.56/41.33 : 1.00/0.00              |    1.094   |      Yes, p =  0.0392      |     1      |[73]ccA>ccN|[2]aTG>aNN,gcC>gcA|[1]aTG>aGC,atG>atT,ATG>CCA,ATG>CCT,AT...|

|    1191    |     1      |    3.312   |             0.23/63.17 : 0.84/0.16              |    3.807   |      Yes, p =  0.0392      |     2      |[78]atC>atN|[74]atA>atN|[2]aaT>aaC|[1]aAt>aGt,aTA>aAT,atA>atC,ATA>GC...|

### ** Found _48_ sites under episodic diversifying positive selection at p <= 0.1**

(base) fred@192 Downloads % 



