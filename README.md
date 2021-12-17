
# Simple Spring Boot application vulnerable to CVE-2021-44228 (Log4Shell)

This proof-of-concept application for CVE-2021-44228 (a.k.a log4shell) is a part of my [writeup](https://www.pidnull.io/2021/12/17/CVE-2021-44228-log4j2-analysis-exploit-PoC.html). For the complete exploit details, refer to the writeup.

## Instructions

Run:

```bash
docker run --rm -p 8080:8080 --name log4shell-poc-app ghcr.io/guerzon/log4shellpoc:latest
```

Or build and run:

```bash
docker build . -t log4shellpoc
docker run --rm -p 8080:8080 --name log4shell-poc-app log4shellpoc
```

## Notes

Spring Boot project inspired by: https://github.com/christophetd/log4shell-vulnerable-app/
