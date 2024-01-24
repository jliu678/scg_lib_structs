# Single Cell Genomics Library Structure
Collections of library structure and sequence of popular single cell genomic methods (mainly scRNA-seq).

## Before you start

Make sure you understand the basic configuration of the Illumina libraries, because most single cell sequencing methods are developed to be sequenced on the Illumina platforms. If you are not familiar with the Illumina sequencing libraries, [click here](https://teichlab.github.io/scg_lib_structs/methods_html/Illumina.html) to check some general information about Illumina library structures and the nature of library preparation.

The HTML pages listed below contain step-by-step procedures of how the libraries are generated experimentally. For the computational preprocessing pipelines for each method, please see this accompanying [__ReadTheDocs documentation__](https://scg-lib-structs.readthedocs.io/en/latest/). For the machine-readable format of the library structure, check [__seqspec__](https://github.com/IGVF/seqspec).

## How to use?

Click the following links to view the methods. Notes:

1. Index1 (i7) is always sequenced using the bottom strand as template, regardless of the Illumina machine in use. That is why the index sequences are reverse complementary to the primer sequences.
2. __IMPORTANT:__ In a dual-index library, how index2 (i5) is sequenced differs from machines to machines. According to the [Index Sequencing Guide](data/indexed-sequencing-overview-guide-15057455-05.pdf) from Illumina, Miseq, Hiseq2000/2500, MiniSeq (Rapid) and NovaSeq 6000 (v1.0) use the bottom strand as template (Forward Strand Workflow), which is why the index sequences are the same as the primer sequences in those machines. iSeq 100, MiniSeq, NextSeq, HiSeq X, HiSeq 3000/4000 and NovaSeq 6000 (v1.5) use the top strand as template (Reverse Complement Workflow), which is why the index sequences are reverse-complementary to the primer sequences in those machines. __All methods listed below use iSeq 100, MiniSeq (Standard), NextSeq, HiSeq X, HiSeq 3000/4000 and NovaSeq 6000 (v1.5) as examples, because this configuration is more frequently used nowadays.__

- ### Gene expression

  - [SMART-seq family (including SMART-seq, SMART-seq2 and SMART-seq3)](https://teichlab.github.io/scg_lib_structs/methods_html/SMART-seq_family.html)
  - [STRT-seq family (including STRT-seq, STRT-seq-C1 and STRT-seq-2i)](https://teichlab.github.io/scg_lib_structs/methods_html/STRT-seq_family.html)
  - [Quartz-seq family (including Quartz-seq and Quartz-seq2)](https://teichlab.github.io/scg_lib_structs/methods_html/Quartz-seq_family.html)
  - [CEL-seq family (including CEL-seq and CEL-seq2)](https://teichlab.github.io/scg_lib_structs/methods_html/CEL-seq_family.html)
  - [10x Chromium Single Cell 3' V3 FeatureBarcoding](https://teichlab.github.io/scg_lib_structs/methods_html/10xChromium3fb.html)
  - 10x Chromium Single Cell 3' V2 and V3 GE:[tecihlab webpage](https://teichlab.github.io/scg_lib_structs/methods_html/10xChromium3.html) or [my backup](https://github.com/jliu678/scg_lib_structs/blob/backup_01242024/methods_html/10xChromium3.html)
  - [10x Chromium Single Cell 3' V1 GE](https://teichlab.github.io/scg_lib_structs/methods_html/10xChromium3v1.html)
  - [10x Chromium Single Cell 5' VDJ](https://teichlab.github.io/scg_lib_structs/methods_html/10xChromium5vdjfb.html)
  - [10x Chromium Single Cell 5' GE](https://teichlab.github.io/scg_lib_structs/methods_html/10xChromium5.html)
  - [SureCell 3' WTA for ddSEQ](https://teichlab.github.io/scg_lib_structs/methods_html/SureCell.html)
  - [MARS-seq / MARS-seq2.0](https://teichlab.github.io/scg_lib_structs/methods_html/MARS-seq.html)
  - [SCRB-seq / mcSCRB-seq](https://teichlab.github.io/scg_lib_structs/methods_html/SCRB-seq.html)
  - [Drop-seq / Seq-Well](https://teichlab.github.io/scg_lib_structs/methods_html/Drop-seq.html)
  - [scifi-RNA-seq](https://teichlab.github.io/scg_lib_structs/methods_html/scifi-RNA-seq.html)
  - [Microwell-seq](https://teichlab.github.io/scg_lib_structs/methods_html/Microwell-seq.html)
  - [BD Rhapsody](https://teichlab.github.io/scg_lib_structs/methods_html/BD_Rhapsody.html)
  - [sci-RNA-seq3](https://teichlab.github.io/scg_lib_structs/methods_html/sci-RNA-seq3.html)
  - [sci-RNA-seq](https://teichlab.github.io/scg_lib_structs/methods_html/sci-RNA-seq.html)
  - [HyDrop-RNA](https://teichlab.github.io/scg_lib_structs/methods_html/HyDrop_RNA.html)
  - [Seq-Well S3](https://teichlab.github.io/scg_lib_structs/methods_html/SeqWell_S3.html)
  - [Tang 2009](https://teichlab.github.io/scg_lib_structs/methods_html/tang2009.html)
  - [SPLiT-seq](https://teichlab.github.io/scg_lib_structs/methods_html/SPLiT-seq.html)
  - [VASA-seq](https://teichlab.github.io/scg_lib_structs/methods_html/VASA-seq.html)
  - [PIP-seq](https://teichlab.github.io/scg_lib_structs/methods_html/PIP-seq.html)
  - [inDrop](https://teichlab.github.io/scg_lib_structs/methods_html/inDrop.html)

- ### Chromatin accessibility and protein-DNA interactions

  - [Plate_scATAC-seq and Pi-ATAC-seq](https://teichlab.github.io/scg_lib_structs/methods_html/plate_and_piATAC-seq.html)
  - [10x Chromium Single Cell ATAC](https://teichlab.github.io/scg_lib_structs/methods_html/10xChromium_scATAC.html)
  - [dscATAC-seq/dsciATAC-seq](https://teichlab.github.io/scg_lib_structs/methods_html/dscATAC.html)
  - [scDNase-seq/scMNase-seq](https://teichlab.github.io/scg_lib_structs/methods_html/scDNase_scMNase.html)
  - [sci-ATAC-seq](https://teichlab.github.io/scg_lib_structs/methods_html/sci-ATAC-seq.html)
  - [HyDrop-ATAC](https://teichlab.github.io/scg_lib_structs/methods_html/HyDrop_ATAC.html)
  - [snATAC-seq](https://teichlab.github.io/scg_lib_structs/methods_html/snATAC-seq.html)
  - [scTHS-seq](https://teichlab.github.io/scg_lib_structs/methods_html/scTHS-seq.html)
  - [itChIP-seq](https://teichlab.github.io/scg_lib_structs/methods_html/itChIP-seq.html)
  - [Drop-ChIP](https://teichlab.github.io/scg_lib_structs/methods_html/Drop-ChIP.html)
  - [CoBATCH](https://teichlab.github.io/scg_lib_structs/methods_html/CoBATCH.html)
  - [scDamID](https://teichlab.github.io/scg_lib_structs/methods_html/scDamID.html)
  - [s3-ATAC](https://teichlab.github.io/scg_lib_structs/methods_html/s3-ATAC.html)

- ### Genomic DNA or DNA methylation

  - [scBS-seq](https://teichlab.github.io/scg_lib_structs/methods_html/scBS-seq.html)
  - [MALBAC](https://teichlab.github.io/scg_lib_structs/methods_html/MALBAC.html)
  - [s3-WGS](https://teichlab.github.io/scg_lib_structs/methods_html/s3-WGS.html)
  - [scRRBS](https://teichlab.github.io/scg_lib_structs/methods_html/scRRBS.html)
  - [LIANTI](https://teichlab.github.io/scg_lib_structs/methods_html/LIANTI.html)

- ### Multi-Omics

  - [10x Chromium Single Cell Multiome ATAC + Gene Expression](https://teichlab.github.io/scg_lib_structs/methods_html/10xChromium_multiome.html)
  - [scNOMe-seq/scCOOL-seq](https://teichlab.github.io/scg_lib_structs/methods_html/scNOMe_scCOOL.html)
  - [scDam&T-seq](https://teichlab.github.io/scg_lib_structs/methods_html/scDamT-seq.html)
  - [ISSAAC-seq](https://teichlab.github.io/scg_lib_structs/methods_html/ISSAAC-seq.html)
  - [SHARE-seq](https://teichlab.github.io/scg_lib_structs/methods_html/SHARE-seq.html)
  - [SNARE-seq](https://teichlab.github.io/scg_lib_structs/methods_html/SNARE-seq.html)
  - [scNMT-seq](https://teichlab.github.io/scg_lib_structs/methods_html/scNMT-seq.html)
  - [scM&T-seq](https://teichlab.github.io/scg_lib_structs/methods_html/scMandT.html)
  - [Paired-seq](https://teichlab.github.io/scg_lib_structs/methods_html/Paired-seq.html)
  - [scCAT-seq](https://teichlab.github.io/scg_lib_structs/methods_html/scCAT-seq.html)
  - [scTrio-seq](https://teichlab.github.io/scg_lib_structs/methods_html/scTrio-seq.html)
  - [scMT-seq](https://teichlab.github.io/scg_lib_structs/methods_html/scMT-seq.html)
  - [G&T-seq](https://teichlab.github.io/scg_lib_structs/methods_html/G_and_T_seq.html)
  - [DR-seq](https://teichlab.github.io/scg_lib_structs/methods_html/DR-seq.html)

- ### TODO list:

  - [Trac-looping](https://www.nature.com/articles/s41592-018-0107-y)
  - [MATQ-seq](https://www.nature.com/articles/nmeth.4145)
  - [ASTAR-seq](https://www.biorxiv.org/content/10.1101/829960v1)
  - [Drop scChIP-seq](https://www.nature.com/articles/s41588-019-0424-9)
  - [sci-Plex](https://science.sciencemag.org/content/early/2019/12/04/science.aax6234.full)
  - [sci-CAR-seq](https://science.sciencemag.org/content/361/6409/1380.full)
  - [snmC2T-seq](https://www.biorxiv.org/content/10.1101/2019.12.11.873398v1)
  - [MALBAC-DT](https://www.biorxiv.org/content/10.1101/2019.12.31.892190v1)
  - [GRID-seq](https://www.nature.com/articles/nbt.3968)
  - [ZipSeq](https://www.biorxiv.org/content/10.1101/2020.02.04.932988v1)
  - [PETRI-seq](https://www.biorxiv.org/content/10.1101/866244v1)
  - [microSPLiT](https://www.biorxiv.org/content/10.1101/869248v2)
  - [scCC](https://www.sciencedirect.com/science/article/pii/S009286742030814X)
  - [scSPRITE](https://www.biorxiv.org/content/10.1101/2020.08.11.242081v1)
  - [TEA-seq/ICICLE-seq](https://www.biorxiv.org/content/10.1101/2020.09.04.283887v2)
  - [sci-ATAC-seq3](https://science.sciencemag.org/content/370/6518/eaba7612.long)
  - [s3-ATAC/WGS/GCC](https://www.biorxiv.org/content/10.1101/2021.01.11.425995v1)
  - [hsrChST-seq](https://www.biorxiv.org/content/10.1101/2021.03.11.434985v1)
  - [TIP-seq](https://www.biorxiv.org/content/10.1101/2021.03.17.435909v1)
  - [ECCITE-seq](https://www.nature.com/articles/s41592-019-0392-0)
  - [ASAP-seq/DOGMA-seq](https://www.nature.com/articles/s41587-021-00927-2)
  - [PHAGE-ATAC](https://www.biorxiv.org/content/10.1101/2020.10.01.322420v1)
  - [Spatial-ATAC-seq](https://www.biorxiv.org/content/10.1101/2021.06.06.447244v1)
  - [Spatial C&T](https://www.science.org/doi/10.1126/science.abg7216)
  - [scTEM-seq](https://www.biorxiv.org/content/10.1101/2021.03.25.436351v1)
  - [DBiT-seq](https://www.sciencedirect.com/science/article/pii/S0092867420313908)
  - [scGET-seq](https://www.nature.com/articles/s41587-021-01031-1)
  - [Multi-CUT&Tag](https://www.sciencedirect.com/science/article/pii/S109727652100753X)
  - [MulTI-Tag](https://www.biorxiv.org/content/10.1101/2021.07.08.451691v1)
  - [TIME-seq](https://www.biorxiv.org/content/10.1101/2021.10.25.465725v1)
  - [scSPLAT](https://www.biorxiv.org/content/10.1101/2021.10.14.464375v2)
  - [EpiDamID](https://www.biorxiv.org/content/10.1101/2021.10.26.465688v1)
  - [scRibo-seq](https://www.nature.com/articles/s41586-021-03887-4)
  - [FLASH-seq](https://www.nature.com/articles/s41587-022-01312-3)
  - [Smart-seq3xpress](https://www.nature.com/articles/s41587-022-01311-4)
  - [sc-end5-seq](https://www.biorxiv.org/content/10.1101/2021.04.04.438388v2)
  - [Slide-seq](https://www.science.org/doi/10.1126/science.aaw1219) / [Slide-seqV2](https://www.nature.com/articles/s41587-020-0739-1) / [Slide-DNA-seq](https://www.nature.com/articles/s41586-021-04217-4) / [Slide-tags](https://www.biorxiv.org/content/10.1101/2023.04.01.535228v1)
  - [CoTECH](https://www.nature.com/articles/s41592-021-01129-z)
  - [PairedTag](https://www.nature.com/articles/s41592-021-01060-3)
  - [GoT-ChA](https://www.biorxiv.org/content/10.1101/2022.05.11.491515v1)
  - [Methyl-HiC](https://www.nature.com/articles/s41592-019-0502-z)
  - [SNuBar-ATAC](https://www.sciencedirect.com/science/article/pii/S1097276521007954)
  - [RAISIN RNA-seq & MIRACL-seq](https://www.sciencedirect.com/science/article/pii/S0092867420309946)
  - [Microbe-seq](https://www.science.org/doi/10.1126/science.abm1483)
  - [SEC-seq](https://www.biorxiv.org/content/10.1101/2022.08.25.505190v1)
  - [scONE-seq](https://www.science.org/doi/10.1126/sciadv.abp8901)
  - [BacDrop](https://pubmed.ncbi.nlm.nih.gov/36708705/)
  - [SPEAC-seq](https://www.science.org/doi/10.1126/science.abq4822)
  - [DisCo](https://www.nature.com/articles/s41592-021-01391-1)
  - [spinDrop](https://www.biorxiv.org/content/10.1101/2023.01.12.523500v1)
  - [sciPlex-ATAC-seq](https://www.biorxiv.org/content/10.1101/2023.03.05.531201v1)
  - [FIPRESCI](https://doi.org/10.1186/s13059-023-02893-1)
  - [SCITO-seq](https://www.nature.com/articles/s41592-021-01222-3)
  - [txci-ATAC-seq](https://www.biorxiv.org/content/10.1101/2023.05.11.540245v1)
  - [snRandom-seq](https://www.nature.com/articles/s41467-023-38409-5)
  - [LAST-seq](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-023-03025-5)
  - [GAGE-seq](https://www.biorxiv.org/content/10.1101/2023.07.20.549578v1)
  - [scCARE-seq](https://www.nature.com/articles/s41594-023-01066-9)
  - [HiRES](https://www.science.org/doi/10.1126/science.adg3797)
  - [LiMCA](https://www.researchsquare.com/article/rs-3210240/v1)
  - [nano-CT](https://www.nature.com/articles/s41587-022-01535-4)
  - [NTT-seq](https://www.nature.com/articles/s41587-022-01588-5)
  - [BuTT-seq](https://genesdev.cshlp.org/content/37/9-10/432)
  - [M3-seq](https://www.nature.com/articles/s41564-023-01462-3)
  - [inDrops-2](https://www.biorxiv.org/content/10.1101/2023.09.26.559493v1)
  - [scRCAT-seq](https://www.nature.com/articles/s41467-020-18976-7)
  - [Phospho-seq](https://www.biorxiv.org/content/10.1101/2023.03.27.534442v1.full)
  - [RamDA-seq](https://www.nature.com/articles/s41467-018-02866-0)

## scRNA-seq technical comparisons

**The basic chemistry is very similar, the main differences among those scRNA-seq methods are summarised in the table below. For a detailed discussion, check the text boxes from our review: [From Tissues to Cell Types and Back: Single-Cell Gene Expression Analysis of Tissue Architecture](https://www.annualreviews.org/doi/10.1146/annurev-biodatasci-080917-013452)**

|                                  | Single cell isolation/capture |     Where RT happens     |         2nd strand synthesis        | Full-length cDNA synthesis |                      Barcode addition                     | Pooling before library |  Library amplification | Gene coverage |
|:--------------------------------:|:-----------------------------:|:------------------------:|:-----------------------------------:|:--------------------------:|:---------------------------------------------------------:|:----------------------:|:----------------------:|:-------------:|
|    10x Chromium Single Cell 3'   |            Droplet            |        In droplets       |                 TSO                 |             Yes            |                    Barcoded RT primers                    |           Yes          |           PCR          |       3'      |
|    10x Chromium Single Cell 5'   |            Droplet            |        In droplets       |                 TSO                 |             Yes            |                    Barcoded TSO primers                   |           Yes          |           PCR          |       5'      |
|            BD Rhapsody           |           Nanowells           |    In collection tubes   | Random priming and primer extension |             No             |                    Barcoded RT primers                    |           Yes          |           PCR          |       3'      |
|         CEL-seq/CEL-seq2         |              FACS             |     In 96w/384w wells    |        RNase H and DNA pol I        |             No             |                    Barcoded RT primers                    |           Yes          | In vitro transcription |       3'      |
|             Drop-seq             |            Droplet            |    In collection tubes   |                 TSO                 |             Yes            |                    Barcoded RT primers                    |           Yes          |           PCR          |       3'      |
| Illumina Bio-Rad SureCell 3' WTA |            Droplet            |        In droplets       |        RNase H and DNA pol I        |             No             |                    Barcoded RT primers                    |           Yes          |           PCR          |       3'      |
|              inDrop              |            Droplet            |        In droplets       |        RNase H and DNA pol I        |             No             |                    Barcoded RT primers                    |           Yes          | In vitro transcription |       3'      |
|       MARS-seq/MARS-seq2.0       |              FACS             |     In 96w/384w wells    |        RNase H and DNA pol I        |             No             |                    Barcoded RT primers                    |           Yes          | In vitro transcription |       3'      |
|           Microwell-seq          |           Nanowells           |    In collection tubes   |                 TSO                 |             Yes            |                    Barcoded RT primers                    |           Yes          |           PCR          |       3'      |
|            Quartz-seq            |              FACS             |     In 96w/384w wells    |  PolyA tailing and primer ligation  |      Yes in principle      |            Ligation of barcoded Truseq adapters           |           No           |           PCR          |       3'      |
|            Quartz-seq2           |              FACS             |     In 96w/384w wells    |  PolyA tailing and primer ligation  |      Yes in principle      |                    Barcoded RT primers                    |           Yes          |           PCR          |       3'      |
|            sci-RNA-seq           |           Not needed          |          In situ         |        RNase H and DNA pol I        |             No             | Barcoded RT primers and library PCR with barcoded primers |           Yes          |           PCR          |       3'      |
|           sci-RNA-seq3           |           Not needed          |          In situ         |        RNase H and DNA pol I        |             No             |          Barcoded RT primers and hairpin adapters         |           Yes          |           PCR          |       3'      |
|           scifi-RNA-seq          |     Droplet multiple cells    |          In situ         |                 TSO                 |             Yes            |         Barcoded RT primers and gel bead barcodes         |           Yes          |           PCR          |       3'      |
|        SCRB-seq/mcSCRB-seq       |              FACS             |     In 96w/384w wells    |                 TSO                 |             Yes            |                    Barcoded RT primers                    |           Yes          |           PCR          |       3'      |
|             Seq-Well             |           Nanowells           |    In collection tubes   |                 TSO                 |             Yes            |                    Barcoded RT primers                    |           Yes          |           PCR          |       3'      |
|            Seq-Well S3           |           Nanowells           |    In collection tubes   | Random priming and primer extension |             No             |                    Barcoded RT primers                    |           Yes          |           PCR          |       3'      |
|  SMART-seq/SMART-seq2/SMART-seq3 |      FACS or Fluidigm C1      |     In 96w/384w wells    |                 TSO                 |             Yes            |             Library PCR with barcoded primers             |           No           |           PCR          |  full-length  |
|             SPLiT-seq            |           Not needed          |          In situ         |                 TSO                 |             Yes            |              Ligation of barcoded RT primers              |           Yes          |           PCR          |       3'      |
|             STRT-seq             |              FACS             |     In 96w/384w wells    |                 TSO                 |             Yes            |                    Barcoded TSO primers                   |           Yes          |           PCR          |       5'      |
|            STRT-seq-C1           |          Fluidigm C1          | In microfluidic chambers |                 TSO                 |             Yes            |                  Barcoded Tn5 transposase                 |           No           |           PCR          |       5'      |
|            STRT-seq-2i           |        FACS or dilution       |      In 9600w wells      |                 TSO                 |             Yes            |          Barcoded PCR primers and Tn5 transposase         |           Yes          |           PCR          |       5'      |
|             Tang 2009            |         FACS or manual        |     In 96w/384w wells    |  PolyA tailing and primer extension |      Yes in principle      |               Ligation of barcoded adaptors               |           No           |           PCR          |  Biased to 3' |

## scATAC-seq technical comparisons

**This is basically Table 1 from our scATAC-seq protocol: [A plate-based single-cell ATAC-seq workflow for fast and robust profiling of chromatin accessibility](https://www.nature.com/articles/s41596-021-00583-5)**

|                                  | Tn5 and adaptors | Staring cell number | Tagmentation | Single-cell/nucleus isolation | Library amplification |  Barcode addition  | Throughput |
|:--------------------------------:|:----------------:|:-------------------:|:------------:|:-----------------------------:|:---------------------:|:------------------:|:----------:|
|      sc-ATAC-seq/snATAC-seq      |    Custom-made   |       500,000+      |     Bulk     |        FACS or dilution       |          PCR          | Tn5 + PCR barcodes |   10,000   |
|             scTHS-seq            |    Custom-made   |       500,000+      |     Bulk     |        FACS or dilution       |      IVT and PCR      | Tn5 + PCR barcodes |   10,000   |
| Plate_scATAC-seq and Pi-ATAC-seq |      Nextera     |        5,000+       |     Bulk     |              FACS             |          PCR          |    PCR barcodes    |    1,000   |
|            Fluidigm C1           |      Nextera     |     4,000-20,000    | Single cells |         Microfluidics         |          PCR          |    PCR barcodes    |     100    |
|           Takara ICELL8          |      Nextera     |        16,000       | Single cells |         Microfluidics         |          PCR          |    PCR barcodes    |    1,000   |
|   10x Chromium Single Cell ATAC  |      Nextera     |      800-15,000     |     Bulk     |            Droplets           |          PCR          |    PCR barcodes    |   10,000   |
|        Bio-Rad dscATAC-seq       |      Nextera     |       60,000+       |     Bulk     |            Droplets           |          PCR          |    PCR barcodes    |   10,000   |
|       Bio-Rad dsciATAC-seq       |    Custom-made   |       600,000+      |     Bulk     |            Droplets           |          PCR          | Tn5 + PCR barcodes |   100,000  |

## Motivation

I was a little bit bombarded with all the single cell methods and got completely lost. To help myself understand all of them and future troubleshooting, I start to perform an on-paper library preparation whenever I see a new single cell method.

## Why bother?

Here I borrow from Feyman:

**What I cannot create, I do not understand.**

----

![](data/feyman.jpeg)

## Citation

If you find this repository useful and would like to cite this resource, please consider citing this repo and the `seqspec` preprint together:

```
@misc{xi_chen_teichlabscg_lib_structs_2023,
	title = {Teichlab/scg\_lib\_structs: {Release} 26th {Oct} 2023},
	copyright = {Creative Commons Attribution 4.0 International},
	shorttitle = {Teichlab/scg\_lib\_structs},
	url = {https://zenodo.org/doi/10.5281/zenodo.10042390},
	abstract = {This is the first release to get a DOI so that people can cite the repo.},
	urldate = {2023-10-26},
	publisher = {Zenodo},
	author = {Xi Chen and Patrick Roelli and Darío Hereñú and Pontus Höjer and Tim Stuart},
	month = oct,
	year = {2023},
	doi = {10.5281/ZENODO.10042390},
}

@techreport{booeshaghi_machine-readable_2023,
	type = {preprint},
	title = {A machine-readable specification for genomics assays},
	url = {http://biorxiv.org/lookup/doi/10.1101/2023.03.17.533215},
	abstract = {Understanding the structure of sequenced fragments from genomics libraries is essential for accurate read preprocessing. Currently, different assays and sequencing technologies require custom scripts and programs that do not leverage the common structure of sequence elements present in genomics libraries. We present seqspec, a machine-readable specification for libraries produced by genomics assays that facilitates standardization of preprocessing and enables tracking and comparison of genomics assays. The specification and associated seqspec command line tool is available at https://github.com/IGVF/seqspec.},
	language = {en},
	urldate = {2023-10-26},
	institution = {Bioinformatics},
	author = {Booeshaghi, A. Sina and Chen, Xi and Pachter, Lior},
	month = mar,
	year = {2023},
	doi = {10.1101/2023.03.17.533215},
}
```

## Feedback

I would be very happy if you go through them and let me know what you think. If you spot some errors/mistakes, or I've missed some key methods. Feel free to raise an issue in the [GitHub repository](https://github.com/Teichlab/scg_lib_structs/issues), or contact me directly:

Xi Chen  
chenx9@sustech.edu.cn
