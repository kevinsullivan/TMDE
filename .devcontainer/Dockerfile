# Copyright © 2001 by the Rectors and Visitors of the University of Virginia. 

# Extend Ubunto 20.04
# FROM ubuntu:20.04
FROM docker.io/kevinsullivan/leanvm 

# Create image without any user interaction
ENV DEBIAN_FRONTEND=noninteractive
RUN echo 'debconf debconf/frontend select Noninteractive' | debconf-set-selections

# Your extensions, if any, here
#
