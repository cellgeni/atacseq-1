From:nfcore/base
Bootstrap:docker

%labels
    MAINTAINER Harshil Patel <harshil.patel@crick.ac.uk>
    DESCRIPTION Singularity image containing all requirements for nf-core/atacseq pipeline
    VERSION 1.0dev

%environment
    PATH=/opt/conda/envs/nf-core-atacseq-1.0dev/bin:$PATH
    export PATH

%files
    environment.yml /

%post
    /opt/conda/bin/conda env create -f /environment.yml
    /opt/conda/bin/conda clean -a
