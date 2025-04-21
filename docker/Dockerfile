# syntax=docker/dockerfile:1
FROM rockylinux:9 AS base
# FROM ubuntu AS base
# COPY setup_tempo.sh setup_tempo.sh
RUN echo "base"

FROM base AS stage1
# COPY setup_tempo2.sh $HOME/setup_tempo2.sh
RUN echo "stage1"

FROM base AS stage2
RUN echo "stage2"
# COPY ./entrypoint.sh /opt/docker/bin/entrypoint
RUN ls -l /opt/docker/bin/entrypoint
ENTRYPOINT ["/opt/docker/bin/entrypoint"]
