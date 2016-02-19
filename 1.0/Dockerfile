FROM golang:latest

ENV HTWTXT_VERSION 1.0.5

WORKDIR $GOPATH/src/

COPY ./htwtxt-${HTWTXT_VERSION}.tar.gz ./
RUN tar xf htwtxt-${HTWTXT_VERSION}.tar.gz
RUN go get htwtxt-${HTWTXT_VERSION}

RUN mkdir ~/htwtxt

EXPOSE 8000

CMD ["htwtxt"]
