start-dfs.sh
start-yarn.sh

hdfs dfs -mkdir /mydata

echo "Hello, this is my first Hadoop file!" > example.txt

hdfs dfs -put example.txt /mydata/

hdfs dfs -ls /mydata

hdfs dfs -cat /mydata/example.txt

hdfs dfs -rm /mydata/example.txt

hdfs dfs -rm -r /mydata

$HADOOP_HOME/sbin/stop-dfs.sh
$HADOOP_HOME/sbin/stop-yarn.sh
