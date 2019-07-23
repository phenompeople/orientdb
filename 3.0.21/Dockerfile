FROM phenompeople/oraclejre
LABEL maintainer="rajesh.jonnalagadda@phenompeople.com" \
	  version="3.0.21" \
	  project="orientdb"
EXPOSE 2424 2480
ARG ORIENTDB_VERSION=3.0.21
RUN wget -q -O /tmp/orientdb.tar.gz "https://s3.us-east-2.amazonaws.com/orientdb3/releases/${ORIENTDB_VERSION}/orientdb-${ORIENTDB_VERSION}.tar.gz" && \
    tar -xzf /tmp/orientdb.tar.gz -C /usr/local && \
    ln -sf /usr/local/orientdb-${ORIENTDB_VERSION} /usr/local/orientdb
