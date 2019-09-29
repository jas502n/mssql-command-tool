# mssql 终端连接工具|命令执行

![](./whoam.png)

## Example
```
./mssql-command-tool-mac -s 10.10.10.10 -u sa -p jas502n -P 1433 -c "whoami"                                                                                                          
nt service\mssqlserver


/mssql-command-tool-mac -s 10.10.10.10 -u sa -p jas502n -P 1433 -c "net user"

\\ 的用户帐户

-------------------------------------------------------------------------------
Administrator            flag                     Guest
命令运行完毕，但发生一个或多个错误。

```

## help

```
NAME:
   Mssql Toolkit - mssql command tool

USAGE:
   mssql-command-tool-mac [global options] command [command options] [arguments...]

VERSION:
   1.0

AUTHOR:
   lostwolf <linuxseclab@gmail.com>

COMMANDS:
   help, h  Shows a list of commands or help for one command

GLOBAL OPTIONS:
   --server value, --host value, -s value  The database server (default: "127.0.0.1")
   --user value, -u value                  The database user (default: "sa")
   --password value, -p value              The database password
   --port value, -P value                  The database port (default: 0)
   --query value, --sql value, -q value    SQL query (default: "select @@version")
   --exec value, -c value, --cmd value     Exec System Command (default: "whoami")
   --debug, -d                             Debug info
   --enable, -e                            Enabled xp_cmdshell
   --help, -h                              show help
   --version, -v                           print the version
```

## 参考链接

https://github.com/Mayter/mssql-command-tool

http://wolvez.club/2019/09/19/mssql-command-tool/
