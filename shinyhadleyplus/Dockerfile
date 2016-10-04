FROM mingjerli/shinyhadleyverse

MAINTAINER Ming-Jer Lee "mingjerli@gmail.com"

# Download and install dependency packages
RUN  R -e "install.packages(c('shinyBS', 'shinythemes','treemap','networkD3','xts','dygraphs','glmnet','reshape'), repos='https://cran.rstudio.com/')" && \
     R -e "devtools::install_github('timelyportfolio/d3treeR')"

EXPOSE 3838

#ENTRYPOINT ["/usr/bin/shiny-server.sh"]
#CMD ["/usr/bin/shiny-server.sh"]