# hadoop-spark-opt

## Setup
Follow the steps in the two links below to setup Hadoop and Spark
1. [Link1](http://www.praveenkumarg.com/install-hadoop-with-spark-on-windows-in-just-5-steps/)
2. [Link2](https://dev.to/awwsmm/installing-and-running-hadoop-and-spark-on-windows-33kc)

## Startup Hadoop
```
start-dfs.cmd && start-yarn.cmd
```

## Web Interfaces

- Resource Manager: http://localhost:8088
- Web UI of the NameNode daemon: http://localhost:50070
- HDFS NameNode web interface: http://localhost:8042

## Useful commands

### Upload data from local system to HDFS
```
fs put --from source_path_and_file --to dest_path_and_file
```

### Download data from HDFS to local system
```
fs get --from source_path_and_file --to dest_path_and_file
```

### Startup Spark Shell
```
spark-shell.cmd
```

### Loading data from HDFS into Spark Shell
```
 scala> val data = sc.textFile("hdfs://localhost:9000/folder/data.txt")
```
