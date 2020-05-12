FROM node:alpine as builder
COPY . .
ENV API_URL=http://localhost:8000
RUN npm install && \
    npm run build

FROM node:alpine as app
COPY --from=builder /dist /dist
RUN npm install -g serve
EXPOSE 5000
CMD ["serve", "-s", "-l", "5000", "dist"]