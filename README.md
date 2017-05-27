please use following command:
docker run --restart=unless-stopped  -e INTERFACE="ens32" -e STATE="BACKUP"   -e          VIRTUAL_ROUTER_ID="51"     -e        PRIORITY="100"       -e      VIRTUAL_IP="192.168.101.200"         -e     VIRTUAL_MASK="24"    -d      -v /root/keep-haproxy/haproxy.cfg:/usr/local/etc/haproxy/haproxy.cfg:ro    --net=host    --privileged      10.0.2.50/winhong/docker-keepalived-haproxy:20170522-2       
-f, /usr/local/etc/haproxy/haproxy.cfg

or use d2.yml
