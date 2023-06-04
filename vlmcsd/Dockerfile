FROM alpine:latest

LABEL version="vlmcsd-1113-2020-03-28-Hotbird64"
LABEL binaries="Linux/intel/static/vlmcsd-x64-musl-static"

WORKDIR /app
COPY vlmcsd-x64-musl-static /app/vlmcsd

EXPOSE 1688/tcp

CMD [ "/app/vlmcsd", "-d", "-D", "-u 1028", "-g 1028"]

# docker build -f ./Dockerfile -t vlmcsd:1113-2020-03-28-Hotbird64-x64-musl-static .
# docker run -d -m 128m --publish 1688:1688  --name vlmcsd vlmcsd:1113-2020-03-28-Hotbird64-x64-musl-static