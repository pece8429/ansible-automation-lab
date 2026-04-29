FROM debian:bookworm

RUN apt update && apt install -y openssh-server python3 sudo && \
    mkdir /var/run/sshd && \
    useradd -m -s /bin/bash ansible && \
    echo "ansible:ansible" | chpasswd && \
    usermod -aG sudo ansible && \
    echo "ansible ALL=(ALL) NOPASSWD:ALL" > /etc/sudoers.d/ansible

EXPOSE 22
CMD ["/usr/sbin/sshd", "-D"]
