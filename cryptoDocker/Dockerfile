FROM ubuntu:16.04

RUN apt-get update
RUN apt-get install -y build-essential libtool autotools-dev autoconf libssl-dev libboost-all-dev software-properties-common python-software-properties
RUN add-apt-repository ppa:bitcoin/bitcoin

RUN apt-get update
RUN apt-get install -y bitcoind
RUN mkdir ~/.bitcoin/ && cd ~/.bitcoin/



COPY bitcoin.conf ~/.bitcoin/

CMD ["bitcoind"]