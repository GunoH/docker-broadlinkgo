FROM golang:alpine

# Packages
RUN \
  apk add git && \
  go get github.com/GeertJohan/go.rice && \
  go get github.com/GeertJohan/go.rice/rice && \
  go get github.com/GunoH/broadlinkgo


# Build
RUN \
  cd /go/src/github.com/GunoH/broadlinkgo/cmd && \
  rice embed-go && \
  go build -o broadlinkgo

ENTRYPOINT ["/go/src/github.com/GunoH/broadlinkgo/cmd/broadlinkgo"]

EXPOSE 8000
