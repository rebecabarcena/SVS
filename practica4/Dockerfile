FROM eboraas/debian:stable
MAINTAINER Rebeca <rebeca.barcena.o@gmail.com>
RUN cd /home && mkdir SPECweb && cd SPECweb \
&& apt-get update \
&& apt-get install -y wget \
&& wget http://www.atc.unican.es/%7evpuente/SVS/SPECweb2005_ins.tar.bz2 \
&& wget http://www.atc.unican.es/%7evpuente/SVS/jdk-1_5_0_22-linux-amd64.bin \
&& apt-get install bzip2 \
&& mv SPECweb2005_ins.tar.bz2 SPECweb2005_ins.tar \
&& tar -xvf SPECweb2005_ins.tar \
&& chmod +x jdk-1_5_0_22-linux-amd64.bin \
&& yes | ./jdk-1_5_0_22-linux-amd64.bin \
&& export PATH=$PATH:/home/jdk1.5.0_22/bin
