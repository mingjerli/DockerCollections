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
  && rm -rf /tmp/downloaded_packages/ /tmp/*.rds

EXPOSE 3838

