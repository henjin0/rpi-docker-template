FROM ros:eloquent
#FROM balenalib/raspberrypi3-debian:latest

RUN apt-get update -y
RUN apt-get install git -y
RUN apt-get install build-essential -y
RUN apt-get install python3-pip -y
#RUN apt-get install python3-rpi.gpio -y
RUN git clone https://github.com/WiringPi/WiringPi.git && cd WiringPi && ./build
RUN pip3 install pigpio
RUN pip3 install RPi.GPIO

RUN mkdir /share_host

