FROM jeksterslab/dynr-rocker

# add additional packages
ADD tools /usr/src/local/src
RUN chmod 777 /usr/src/local/src/setup.sh && \
    ./usr/src/local/src/setup.sh          && \
    rm -rf /usr/src/local/src

RUN echo 'root:root' | chpasswd

# extra metadata
LABEL author="Ivan Jacob Agaloos Pesigan <learn.jeksterslab@gmail.com>"
LABEL description="jeksterslab/dynr-rocker container."
