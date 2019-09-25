# R-markdown

To be able to use thesisdown (a package for writing and formatting a thesis) you’ll need to follow the steps on this page under the “Using thesisdown from Chester’s GitHub” section: https://github.com/ismayc/thesisdown
 
Also, to create Word documents from Rmarkdown, you’ll need Pandoc installed. I can’t remember exactly where to get it from but either the latest version of Rstudio comes with it or it will tell you where to download it from when you first try to knit to Word.
 
I recommend following the steps in thesisdown, then creating a new template (note: ‘ Name: index’ cannot be changed) and clicking ‘knit’ straight away to see if your computer can create a document. If it can’t, the errors in the console should tell you what software you need to make it work. Unfortunately, downloading thesisdown and bookdown can be an issue on some computers and it might take some troubleshooting to get it to work. If you can’t get it to work then there is still value in coming to the workshop to determine whether you think it is useful and therefore, whether you want to spend the time troubleshooting.

```
# Thesis Down..
install.packages(c('tinytex', 'rmarkdown'))
tinytex::install_tinytex()
# after restarting RStudio, confirm that you have LaTeX with
tinytex:::is_tinytex()
 
# Book down package install
if (!require("remotes")) install.packages("remotes", repos = "http://cran.rstudio.org")
remotes::install_github("rstudio/bookdown")
remotes::install_github("ismayc/thesisdown")
 
#check
library(bookdown)
library(thesisdown)
library(tinytex)
 
# Restart R  - open a new R Markdown file - select from template
#- select the thesis option
#- knit the 'blank' template page that opens.
 
# IF that works, you're done.
```

Download the Writing_in_RMarkdown folder before the workshop
