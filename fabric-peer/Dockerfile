FROM hyperledger/fabric-peer:x86_64-1.1.0-preview
RUN mkdir /host \
 && chown -R :0 /host \
 && chmod -R a+w /host \
 && chown -R :0 /etc/hyperledger \
 && chmod -R a+w /etc/hyperledger
EXPOSE 7051 7053
VOLUME /host/var/run
VOLUME /etc/hyperledger/fabric/msp
#WORKDIR /opt/gopath/src/github.com/hyperledger/fabric/peer
CMD peer node start