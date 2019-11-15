# Centos 7 with Apache Web Server
To build the image
`docker build --rm -t centos-systemd-httpd:7 .`

To run it on Mac use the following command:

    docker run -d -e=container=docker --stop-signal=SIGRTMIN+3 -p 80:80 --tmpfs /tmp --tmpfs /run -v /sys/fs/cgroup:/sys/fs/cgroup:ro centos-systemd-httpd:7

