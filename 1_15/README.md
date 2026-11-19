# Docker Quick Reference

A small Python web application displaying useful Docker commands. Built for
exercise 1.15; it uses the Python standard library without external packages.

## Build and run locally

Run these commands from this directory:

```sh
docker build -t docker-quick-reference .
docker run --rm -p 127.0.0.1:8090:8080 docker-quick-reference
```

Open http://localhost:8090 to view the reference. GET /health returns
`{"status": "ok"}`. The server listens on container port 8080 and runs as
an unprivileged user.
