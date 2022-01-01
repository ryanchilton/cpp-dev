FROM ubuntu:focal

RUN mkdir /code

WORKDIR /code

# set time zone so installation of tzdata package doesn't hang waiting for user input
ENV TZ=America/New_York
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

# install build tools
RUN apt-get update && apt-get -y --no-install-recommends install \
	build-essential \
	cmake \
	gdb \
	libboost-all-dev \
	doxygen






