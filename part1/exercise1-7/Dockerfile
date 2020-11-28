FROM ubuntu:16.04

WORKDIR /mydir
RUN apt-get update && apt-get install -y curl
COPY localScript.sh .
RUN chmod a+x localScript.sh
CMD ["/mydir/localScript.sh"]