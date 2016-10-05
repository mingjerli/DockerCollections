FROM mingjerli/shinyhadleyverse

MAINTAINER Ming-Jer Lee "mingjerli@gmail.com"

# Download and install dependency packages
RUN install2.r --error -l /usr/lib/R/site-library -d TRUE\
    shinyBS \
    shinythemes \
    treemap \
    networkD3 \ 
    xts \
    dygraphs \
    glmnet \
    reshape \
  && r -e "remotes::install_github('timelyportfolio/d3treeR', lib='/usr/lib/R/site-library')" \ 
  && rm -rf /tmp/downloaded_packages/ /tmp/*.rds

EXPOSE 3838

