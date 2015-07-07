##Description:
The ZooKeeper service can be monitored in one of two primary ways;

1) the command port through the use of 4 letter words

2) JMX. See the appropriate section for your environment/requirements.

1. zookeeper命令行模式结合telnet或者nc:http://zookeeper.apache.org/doc/r3.4.6/zookeeperAdmin.html#sc_zkCommands

2. 通过JMX监控zookeeper:http://zookeeper.apache.org/doc/r3.4.6/zookeeperJMX.html

##模板使用方法:
Monitoring zookeeper remotely on zabbix server.

1.upload getZookeeperInfo.py to externalscripts folder. A chmod/chown to get execution permission is necessary.

2.import the template and linked to the host.

##Macros

You don't need to modify the template if you are using the standard port to access to the zookeeper (port 2181).
If you need a different zookeeper port for the monitor, you will need to modify the {$ZOOKEEPERPORT} macro.

##Triggers

There are 2 trigger to detect zookeeper port issues.

##Graphs

There is a graph of zookeeper received packets and sended packets.


##Contributors:

* [xiaobao623 ] (https://github.com/xiaobao623)
