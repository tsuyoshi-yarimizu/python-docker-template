FROM python:3.9

RUN apt update
RUN apt -y upgrade
RUN apt -y install apt-utils

RUN apt -y install locales && \
    localedef -f UTF-8 -i ja_JP ja_JP.UTF-8
ENV LANG ja_JP.UTF-8
ENV LANGUAGE ja_JP:ja
ENV LC_ALL ja_JP.UTF-8
ENV TZ JST-9
ENV TERM xterm

RUN apt install -y vim less

RUN pip install --upgrade pip
RUN pip install --upgrade setuptools

