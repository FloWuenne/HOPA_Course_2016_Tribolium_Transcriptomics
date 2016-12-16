#INFO
This page is thought to be supplemental information to the analysis of the Tribolium Transcriptomics group from the HOPA 2016 Course (University of Muenster). On this page, information regarding the data analysis that is supplied in the github repository.

# Interactive sleuth analysis
Currently, due to software incompatabilities on the shinyapps.io server, we were unable to host the interactive shiny analysis of the data online. However the .rds objects that are supplied in the folder [shiny_rds_objects](https://github.com/FloWuenne/HOPA_Course_2016_Tribolium_Transcriptomics/tree/master/shiny_rds_objects), can be downloaded and used in Rstudio to create a local shiny object. To open an interactive sleuth server on your local machine, download the rds object and perform the following in RStudio. (This requires sleuth to be installed on your machine. If you do not have sleuth installed, visit this page: http://pachterlab.github.io/sleuth/download)

    library(sleuth)
    so <- readRDS("YOUR_RDS_FILE.rds")
    shiny_live(so)



# Quality Control files

