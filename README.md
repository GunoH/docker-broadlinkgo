# Broadlinkgo in docker container

## Getting started

Clone the repo, and then:

```bash
cd dockerfile
docker build -t broadlinkgo .
docker run -itd --name broadlinkgo -p8000:8000 broadlinkgo
```

Now visit http://localhost:8000 in your browser.
