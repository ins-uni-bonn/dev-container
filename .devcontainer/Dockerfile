FROM ubuntu:jammy

RUN apt-get update && DEBIAN_FRONTEND=noninteractive TZ=Europe/Berlin apt-get install -y curl build-essential clang clang-format gdb cmake-curses-gui ninja-build git python3 python3-dev python3-matplotlib python3-numpy python3-scipy pybind11-dev openmpi-bin libopenmpi-dev dotnet-sdk-6.0 dotnet-runtime-6.0 && apt-get clean
RUN update-alternatives --install /usr/bin/cc cc /usr/bin/clang 100 && update-alternatives --install /usr/bin/c++ c++ /usr/bin/clang++ 100

ENV OMPI_ALLOW_RUN_AS_ROOT=1
ENV OMPI_ALLOW_RUN_AS_ROOT_CONFIRM=1