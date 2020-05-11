FROM alpine:3.7 

ENV LC_ALL=C.UTF-8 

RUN apk add --no-cache curl python ca-certificates && \ 
    curl -L https://yt-dl.org/downloads/latest/youtube-dl -o /usr/local/bin/youtube-dl && \ 
    chmod a+x /usr/local/bin/youtube-dl && \ 
    apk del curl && \ 
    adduser -D app 

USER app 

WORKDIR /app 

ENTRYPOINT ["/usr/local/bin/youtube-dl"] 