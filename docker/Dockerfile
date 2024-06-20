FROM ubuntu:24.04

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get update \
    && apt-get install -y \
      gimp \
    && rm -rf /var/lib/apt/lists/*

CMD ["gimp"]

# CMD ["/bin/bash"]