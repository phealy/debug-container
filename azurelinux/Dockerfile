FROM mcr.microsoft.com/cbl-mariner/base/core:2.0
RUN tdnf install -y cri-tools dnf ebtables gawk bind-utils iperf3 iptables iproute iputils man nftables nmap nmap-ncat perl python3 python3-pip tcpdump util-linux vim && tdnf clean all
RUN tdnf makecache # Since this will be updated daily, this will make installs faster
CMD ["/bin/sh", "-c", "echo \"This is a debug pod; it takes no actions beside sleeping. If you're running this under docker, press ctrl-p ctrl-q to escape.\"; exec sleep infinity"]
