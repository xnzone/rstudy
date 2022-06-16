FROM rocker/rstudio:3.6.3-ubuntu18.04

RUN apt-get update \
    && apt-get install -y --no-install-recommends \
    libxml2-dev libz-dev tzdata cmake # add any additional libraries you need

CMD ["/init"]

COPY ./install-scripts/geo-install-packages.R /home/rstudio/geo-install-packages.R

# RUN Rscript /home/rstudio/geo-install-packages.R
