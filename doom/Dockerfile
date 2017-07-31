FROM arm32v7/debian:stretch-slim

RUN apt-get -yqq update && apt-get install --no-install-recommends -y \
        libgl1-mesa-dri chocolate-doom doom-wad

ADD startdoom.sh /

CMD ["/bin/sh", "/startdoom.sh"]
