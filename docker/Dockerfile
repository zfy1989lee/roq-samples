FROM frolvlad/alpine-miniconda3
MAINTAINER Hans Erik Thrane <info@roq-trading.com>

COPY pkgs/ /pkgs/
RUN conda install --quiet --yes --override-channels --channel file:///pkgs --channel defaults roq-samples

ENTRYPOINT [ "/opt/conda/bin/roq-samples-example-1" ]
CMD        [ "--help" ]
