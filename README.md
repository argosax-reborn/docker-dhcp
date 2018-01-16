Docker-DHCP
-------------------------------
From Majes For Vpnwall Services


How to use :
------------

create data/dhcpd.conf with a subnet clause for the specified network interface of the machine running docker

start the container with the --net=host option and specify interface to run the dhcp on

run docker run -it --rm --net=host -v '$(pwd)/data':/data networkboot/dhcpd eth0'

use ctrl+c to stop it

start with simply run option to iterate though options
