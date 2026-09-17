FROM dorowu/ubuntu-desktop-lxde-vnc

USER root
RUN apt-get update && apt-get install -y firefox && \
    mkdir -p /home/ubuntu/Desktop && \
    echo '[Desktop Entry]\nName=CrazyGames Dev\nExec=firefox https://developer.crazygames.com/\nType=Application\nIcon=firefox' > /home/ubuntu/Desktop/crazygames.desktop && \
    chmod +x /home/ubuntu/Desktop/crazygames.desktop && \
    chown -R ubuntu:ubuntu /home/ubuntu/Desktop && \
    rm -rf /var/lib/apt/lists/*

ENV RESOLUTION=1280x800
EXPOSE 6080 5901
