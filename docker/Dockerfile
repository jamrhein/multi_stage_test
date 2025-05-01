# syntax=docker/dockerfile:1
FROM rockylinux:9 AS base
# FROM ubuntu AS base
RUN find / -name Dockerfile
RUN pwd
RUN ls -l 
COPY setup_tempo.sh setup_tempo.sh
RUN echo "base"
RUN ls -l 

FROM base AS stage1
COPY setup_tempo2.sh setup_tempo2.sh
# COPY entrypoint.sh /opt/docker/bin/entrypoint
RUN ls -l
RUN echo "stage1"
# RUN ls -l /opt/docker/bin/entrypoint
# ENTRYPOINT ["/opt/docker/bin/entrypoint"]
