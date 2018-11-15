# MapR Support Dump eXtractor

1. fix shebang to python3
```bash
#!/usr/local/bin/python3
```
2. run this script with support dump
```bash
$ ./msdx mysupport-output-1.tar
```

Sample output
```
OS : CentOS Linux release 7.5.1804 (Core)


Logs found
misc-Nov-14-1701/logs/mapr-logs/mfs.log-3
misc-Nov-14-1701/logs/mapr-logs/warden.log.1
misc-Nov-14-1701/logs/mapr-logs/warden.log
misc-Nov-14-1701/logs/mapr-logs/cldb.log
misc-Nov-14-1701/logs/mapr-logs/apiserver/apiserver.out
misc-Nov-14-1701/logs/mapr-logs/apiserver/apiserver.log
misc-Nov-14-1701/logs/drill-1.14.0/drillbit.log


ERROR and FATAL counts
mfs                      ERROR:47, FATAL:0
warden                   ERROR:13, FATAL:0
cldb                     ERROR:251, FATAL:0
apiserver                        ERROR:23, FATAL:0
drill                    ERROR:0, FATAL:0


START/END records
2018-11-14 00:43:37.174000      mfs on
2018-11-14 00:43:40.804000      mfs off
2018-11-14 01:00:21.919000 warden on
2018-11-14 01:00:23.998000      mfs on
2018-11-14 01:00:37.154000      cldb on
2018-11-14 01:01:18.700000              apiserver on
2018-11-14 01:01:24.145000              drill on
2018-11-14 02:57:52.373000              drill off
2018-11-14 02:58:09.668000              drill on


ifconfig network failure detection


Netstat check
Ip:
Icmp:
Tcp:
Udp:
UdpLite:
TcpExt:
    1 times recovered from packet loss by selective acknowledgements
IpExt:


Firewall check
firewalld is NOT working
```
