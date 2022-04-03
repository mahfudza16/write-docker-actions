FROM golang:1.15
WORKDIR /go/src/hello
COPY . .
RUN go get -d -v ./...
ENV GOBIN=$GOPATH/bin
ENV PATH=$PATH:$GOBIN
RUN go install -v ./...
CMD ["hello"]
