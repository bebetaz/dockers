FROM fuyaode/android-19

MAINTAINER bebetaz

RUN apt-get update && \
    apt-get install -y openssh-server && \
    apt-get clean && \
    apt-get autoclean

EXPOSE 7474
COPY RMBridge_1.2.0.apk RMBridge_1.2.0.apk
COPY droid-VNC-server.apk droid-VNC-server.apk
COPY install.sh ./install.sh
RUN chmod +x ./install.sh
CMD ["./install.sh"]
