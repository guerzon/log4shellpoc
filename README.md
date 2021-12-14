
# Simple Spring Boot application vulnerable to CVE-2021-44228 (Log4Shell)

This proof-of-concept application for CVE-2021-44228 (a.k.a log4shell) is a part of [writeup in-progress]. For the complete exploit details, refer to the writeup.

## Instructions

Build:

```bash
docker build . -t log4shellpoc-app
```

Run:

```bash
docker run --rm -p 8080:8080 --name lo4shell-poc-app localhost/log4shellpoc-app
```
