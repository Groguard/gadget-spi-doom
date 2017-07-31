FROM arm32v7/debian:stretch-slim

# Add non-free to source list
RUN sed -i 's/main/main non-free/' /etc/apt/sources.list

# Update and download doom files
RUN apt-get -yqq update && apt-get install --no-install-recommends -y \
        libgl1-mesa-dri prboom-plus doom-wad-shareware

# Add the script to run doom
ADD startdoom.sh /

# Run the script
CMD ["/bin/sh", "/startdoom.sh"]
