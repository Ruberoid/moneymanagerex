FROM ubuntu:zesty
MAINTAINER developers@moneymanagerex.org
RUN sed -i -re 's/(([a-z]{2}\.)?archive|security)\.ubuntu\.com/old-releases.ubuntu.com/g' /etc/apt/sources.list && \
    apt-get update && \
    apt-get install -y --no-install-recommends \
      cmake build-essential gettext git pkg-config lsb-release \
      libwxgtk3.0-dev libwxgtk-webview3.0-dev \
      libwxsqlite3-3.0-dev liblua5.2-dev \
      automake libtool ccache && \
    apt-get clean
