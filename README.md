# fullcycle-service-discovery


## consul agent -dev
run consul as dev mode

## consul agent -server -bootstrap-expect=3 -bind=172.20.0.3 -data-dir=/var/lib/consul -config-dir=/etc/consul.d -node=consulserver01
run in server mode expecting 3 other servers to connect, bind to container ip, say where consul is going to save its files and consul config files

# consul agent -bind=172.20.0.3 -data-dir=/var/lib/consul -config-dir=/etc/consul.d -node=consulclient01
without any specific flag it will be created as a client consul

# consul reload

# consul catalog nodes -service nginx
say which server service nginx is registred
# dig @localhost -p 8600
connect to consul using DNS
