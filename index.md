
# INFO
This page is thought to be supplemental data to the analysis of the Tribolium Transcriptomics group from the HOPA 2016 Course (University of Muenster). This page serves mainly as a hub for the Sleuth shiny server that provide interactive analysis of the RNA-seq data. On this page you will be able to find the analysis for the 6h timepoint. The 18h timepoints were not uploaded due to limited instances allowed by shinyapps.io in the free version. Please be aware, that shinyapps.io does only allow 25h of active usage for each server under the free license so if a server can't be reached it might be that the data limit for the moth is reached!

## Links to Sleuth Shiny Server

To open the interactive shiny Server for the comparison of each condition  VS the naive control, just click the sample names below. 

**Please be aware that due to the free nature of shinyapps.io and the size of the analysis, loading the page might take up to 3 minutes. Afterwards the app should be quickly responsive however! So remember, please be patient!**

## Cro1
* [Cro1_BttO_6h vs Cro1_NC_6h]()
* [Cro1_BttP_6h vs Cro1_NC_6h]()
* [Cro1_PC_6h vs Cro1_NC_6h]()

## SB
* [SB_BttO_6h vs SB_NC_6h](https://flowuenne.shinyapps.io/sb_bttp_6h/)
* [SB_BttP_6h vs SB_NC_6h]()
* [SB_PC_6h vs SB_NC_6h]()

# Interactive sleuth analysis
The .rds objects that are supplied in the folder [shiny_rds_objects](https://github.com/FloWuenne/HOPA_Course_2016_Tribolium_Transcriptomics/tree/master/shiny_rds_objects), can be downloaded and used in Rstudio to create a local shiny object. To open an interactive sleuth server on your local machine, download the rds object and perform the following in RStudio. (This requires sleuth to be installed on your machine. If you do not have sleuth installed, visit this page: http://pachterlab.github.io/sleuth/download)

    library(sleuth)
    so <- readRDS("YOUR_RDS_FILE.rds")
    shiny_live(so)

# Quality Control files

All compiled MultiQC reports for the analysis can be found in the folder: MultiQC_Reports

SB: laboratory strain
Cro1: wildtype strain
pretrimmed: quality analysis of raw data
posttrimmed: quality analysis of edited data
STAR: controll of STAR files (how many alignments etc.)
