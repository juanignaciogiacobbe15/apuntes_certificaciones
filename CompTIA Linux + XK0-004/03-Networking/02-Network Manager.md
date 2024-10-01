# Network Manager

- The NetworkManager command line Interface.


> [!NOTE] `nmcli`
> This is the command line utility used for configuring network devices and their connection settings.


> [!NOTE] `nmcli dev`
> This is short for 'device' which is the physical hardware(such as network interface card) that we use to connect to a network.


> [!NOTE] `nmcli con`
> This is short of 'connection' which contains the network configuration settings assigned to a particular device. We assign our IP address and DNS settings to a connection.


![](../img/Pasted%20image%2020240924101425.png)


> [!NOTE] `ip`
> This command can modify IP address settings, route settings and show interface statistics. This is from the iproute2 project.

- `ip addr show` displays IP address information.
- `ip route show` displays the routing table.
- `ip -s addr` show statistics on configured interfaces.

- Command that is used to persistently configure the computer's host name.