  
FROM alpine

WORKDIR /usr/app

COPY . .

RUN apk add --no-cache git nodejs nodejs-npm && \
    npm install && \
    npm run build

CMD npm start