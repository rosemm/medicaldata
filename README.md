
<!-- README.md is generated from README.Rmd. Please edit that file -->

# medicaldata <img src='man/figures/hex-medicaldata.png' align="right" height="240">

## Overview

This is a data package with 15 medical datasets for teaching
Reproducible Medical Research with R. The link to the pkgdown reference
website for {medicaldata} is
[here](https://higgi13425.github.io/medicaldata/) and in the links at
the right. This package will be useful for anyone teaching R to medical
professionals, including doctors, nurses, trainees, and students. <br>
<br> These datasets range from reconstructed versions of James Lind’s
scurvy dataset (1757) and the original Streptomycin for Tuberculosis
trial (1948), a 2012 RCT of indomethacin to prevent post-ERCP
pancreatitis that I was involved in, to cohort data on SARS-CoV2 testing
results (2020). Many of the datasets come from the American Statistical
Association’s TSHS (Teaching Statistics in the Health Sciences)
[Resources Portal](https://www.causeweb.org/tshs/category/dataset/),
maintained by [Carol
Bigelow](https://www.umass.edu/sphhs/person/carol-bigelow) at the
University of Massachusetts (with permission). A growing number of
datasets in the dev version were generously donated by [Frank
Harrell](https://www.fharrell.com) from his website
[here](https://hbiostat.org/data/). These datasets are currently only in
the dev version of the package on github.com, which should make it to
CRAN in January 2022.

## How to Install and Use {medicaldata} Datasets

1.  Install the stable, current CRAN version with
    `install.packages("medicaldata")`. If you want to try out the
    in-development version (which may have new datasets and vignettes,
    but which may also be intermittently wonky), install with:
    `remotes::install_github("higgi13425/medicaldata")`

2.  Then load the package with `library(medicaldata)`

3.  Then you can list the datasets available with
    `data(package = "medicaldata")`

4.  Then assign a particular dataset to a named object in your
    environment with: <br> `covid <- medicaldata::covid_testing` <br>
    where `covid` is the name of the new object, and `covid_testing` is
    the name of the dataset.<br>

5.  Articles (vignettes) on how to use the datasets can be found at the
    pkgdown [website](https://higgi13425.github.io/medicaldata/) under
    the **Articles** tab.

6.  You can click on the links below to view the description document
    and/or codebook for each dataset. This information is also available
    under the Reference tab above, or within R by using
    `help(dataset_name)`. <br>

## Please Donate Datasets

If you have access to data from a randomized, controlled clinical trial,
or a prospective cohort study, or even a case-control study, please
consider obtaining the appropriate permissions, anonymizing the data,
and donating the dataset for teaching purposes to add to this package.
Open an issue on the github page (source code link at the top right) to
open the discussion of a data donation. I am happy to help with
anonymization.

## List of Datasets

Click on links below for more details about the dataset itself in the
Description Document, and more details about the variables included in
the dataset in the Codebook. Note that each dataset also has a help file
that you can use within R or RStudio, by entering `help("dataset_name")`
in the Console pane.

| Dataset         | Description document                                                                                                                          | Codebook                                                                                                                                         |
|:----------------|:----------------------------------------------------------------------------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| strep_tb        | [strep_tb_desc](https://htmlpreview.github.io/?https://github.com/higgi13425/medicaldata/blob/master/man/description_docs/strep_tb_desc.html) | [strep_tb_codebook](https://htmlpreview.github.io/?https://github.com/higgi13425/medicaldata/blob/master/man/codebooks/strep_tb_codebook.html)   |
| scurvy          | [scurvy_desc](https://htmlpreview.github.io/?https://github.com/higgi13425/medicaldata/blob/master/man/description_docs/scurvy_desc.html)     | [scurvy_codebook](https://htmlpreview.github.io/?https://github.com/higgi13425/medicaldata/blob/master/man/codebooks/scurvy_codebook.html)       |
| indo_rct        | [indo_rct_desc](https://htmlpreview.github.io/?https://github.com/higgi13425/medicaldata/blob/master/man/description_docs/indo_rct_desc.html) | [indo_rct_codebook](https://htmlpreview.github.io/?https://github.com/higgi13425/medicaldata/blob/master/man/codebooks/indo_rct_codebook.html)   |
| polyps          | [polyps_desc](https://htmlpreview.github.io/?https://github.com/higgi13425/medicaldata/blob/master/man/description_docs/polyps_desc.html)     | [polyps_codebook](https://htmlpreview.github.io/?https://github.com/higgi13425/medicaldata/blob/master/man/codebooks/polyps_codebook.html)       |
| covid_testing   | [covid_desc](https://htmlpreview.github.io/?https://github.com/higgi13425/medicaldata/blob/master/man/description_docs/covid_desc.html)       | [covid_codebook](https://htmlpreview.github.io/?https://github.com/higgi13425/medicaldata/blob/master/man/codebooks/covid_testing_codebook.html) |
| blood_storage   | [blood_storage_desc](https://www.causeweb.org/tshs/datasets/Blood%20Storage%20Dataset%20Introduction.pdf)                                     | [blood_storage_codebook](https://www.causeweb.org/tshs/datasets/Blood%20Storage%20Data%20Dictionary.pdf)                                         |
| cytomegalovirus | [cytomegalovirus_desc](https://www.causeweb.org/tshs/datasets/Cytomegalovirus%20Dataset%20Introduction.pdf)                                   | [cytomegalovirus_codebook](https://www.causeweb.org/tshs/datasets/Cytomegalovirus%20Data%20Dictionary.pdf)                                       |
| esoph_ca        | [esoph_ca_desc](https://htmlpreview.github.io/?https://github.com/higgi13425/medicaldata/blob/master/man/description_docs/esoph_ca_desc.html) | [esoph_ca_codebook](https://htmlpreview.github.io/?https://github.com/higgi13425/medicaldata/blob/master/man/codebooks/esoph_ca_codebook.html)   |
| laryngoscope    | [laryngoscope_desc](https://www.causeweb.org/tshs/datasets/Laryngoscope%20Dataset%20Introduction.pdf)                                         | [laryngoscope_codebook](https://www.causeweb.org/tshs/datasets/Laryngoscope%20Data%20Dictionary.pdf)                                             |
| licorice_gargle | [licorice_gargle_desc](https://www.causeweb.org/tshs/datasets/Licorice%20Gargle%20Dataset%20Introduction.pdf)                                 | [licorice_gargle_codebook](https://www.causeweb.org/tshs/datasets/Licorice%20Gargle%20Data%20Dictionary.pdf)                                     |
| opt             | [opt_desc](https://www.causeweb.org/tshs/datasets/OPT_Dataset_Introduction.pdf)                                                               | [opt_codebook](https://www.causeweb.org/tshs/datasets/OPT_Data_Dictionary.pdf)                                                                   |
| cath (dev)      | [cath_desc](https://htmlpreview.github.io/?https://github.com/higgi13425/medicaldata/blob/master/man/description_docs/cath_desc.html)         | [cath_codebook](https://htmlpreview.github.io/?https://github.com/higgi13425/medicaldata/blob/master/man/codebooks/cath_codebook.html)           |
| smartpill       | [smartpill_desc](https://www.causeweb.org/tshs/datasets/Smart%20Pill%20Dataset%20Introduction.pdf)                                            | [smartpill_codebook](https://www.causeweb.org/tshs/datasets/Smart%20Pill%20Data%20Dictionary.pdf)                                                |
| supraclavicular | [supraclavicular_desc](https://www.causeweb.org/tshs/datasets/Supraclavicular%20Dataset%20Introduction.pdf)                                   | [supraclavicular_codebook](https://www.causeweb.org/tshs/datasets/Supraclavicular%20Data%20Dictionary.pdf)                                       |
| indometh        | [indometh_desc](https://htmlpreview.github.io/?https://github.com/higgi13425/medicaldata/blob/master/man/description_docs/indometh_desc.html) | [indometh_codebook](https://htmlpreview.github.io/?https://github.com/higgi13425/medicaldata/blob/master/man/codebooks/indometh_codebook.html)   |
| theoph          | [theoph_desc](https://htmlpreview.github.io/?https://github.com/higgi13425/medicaldata/blob/master/man/description_docs/theoph_desc.html)     | [theoph_codebook](https://htmlpreview.github.io/?https://github.com/higgi13425/medicaldata/blob/master/man/codebooks/theoph_codebook.html)       |

<!-- badges: start -->

[![R-CMD-check](https://github.com/higgi13425/medicaldata/workflows/R-CMD-check/badge.svg)](https://github.com/higgi13425/medicaldata/actions)
<!-- badges: end -->
