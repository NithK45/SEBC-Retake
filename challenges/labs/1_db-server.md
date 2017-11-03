The command hostname -f and its output
```
[root@ip-172-31-44-20 ~]# hostname -f
ip-172-31-44-20.us-west-2.compute.internal

```
The command mysql -u <user> -p<password> -e "status;" and its output

```
[root@ip-172-31-44-20 ~]# mysql -u root -p -e "status;"
Enter password:
--------------
mysql  Ver 14.14 Distrib 5.5.58, for Linux (x86_64) using readline 5.1

Connection id:          3
Current database:
Current user:           root@localhost
SSL:                    Not in use
Current pager:          stdout
Using outfile:          ''
Using delimiter:        ;
Server version:         5.5.58 MySQL Community Server (GPL)
Protocol version:       10
Connection:             Localhost via UNIX socket
Server characterset:    latin1
Db     characterset:    latin1
Client characterset:    utf8
Conn.  characterset:    utf8
UNIX socket:            /var/lib/mysql/mysql.sock
Uptime:                 3 min 33 sec

Threads: 1  Questions: 16  Slow queries: 0  Opens: 33  Flush tables: 1  Open tables: 26  Queries per second avg: 0.075
--------------

```

The command mysql -u <user> -p<password> -e "show databases;" and its output
```
[root@ip-172-31-44-20 ~]# mysql -u root -p -e "show databases;"
Enter password:
+--------------------+
| Database           |
+--------------------+
| information_schema |
| hive               |
| hue                |
| mysql              |
| oozie              |
| performance_schema |
| rman               |
| scm                |
| sentry             |
| test               |
+--------------------+
```
