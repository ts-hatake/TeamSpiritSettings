FROM salesforce/salesforcedx:latest-slim

RUN apt update && apt install -y \
  ant \
  subversion

COPY ant-salesforce.jar /usr/share/ant/lib

RUN apt install -y language-pack-ja-base language-pack-ja locales
RUN locale-gen ja_JP.UTF-8
ENV LANG ja_JP.UTF-8
