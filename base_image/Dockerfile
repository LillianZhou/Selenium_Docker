FROM selenium/standalone-chrome
USER root
ARG https_proxy
ARG http_proxy

RUN apt-get update
# Install required libraries
RUN apt-get install -yq python
RUN apt-get update && apt-get install -yq --no-install-recommends python-pip
RUN pip -v
RUN pip install --no-cache-dir virtualenv
RUN pip install selenium==3.3.1
RUN pip install pytest==3.5.0



