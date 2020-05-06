FROM quay.io/eclipse/che-nodejs8-centos:nightly as node-frontend-dev
COPY --chown=10001:10001 . /projects/postit-app/node-frontend
WORKDIR /projects/postit-app/node-frontend
RUN env && \
    npm install && \
    tar zcvf node_modules.tar.gz node_modules