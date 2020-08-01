FROM ubuntu:16.04 

WORKDIR /mydir 
RUN apt-get update && apt-get install -y curl wget

COPY curler.sh .

RUN chmod +x curler.sh

CMD ["/mydir/curler.sh"]
