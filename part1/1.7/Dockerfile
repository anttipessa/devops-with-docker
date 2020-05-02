FROM ubuntu:16.04 

RUN apt-get update && apt-get install -y curl wget 
COPY script.sh .

CMD ["/bin/bash","script.sh"]