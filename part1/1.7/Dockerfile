FROM ubuntu:16.04 

RUN apt-get update
RUN apt-get install -y curl
RUN apt-get install -y bash

WORKDIR \mydir 
COPY start.sh . 
RUN chmod +x start.sh

CMD ["/bin/bash"]