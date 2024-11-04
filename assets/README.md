# 算法说明
从HDFS获取csv样本文件（从实网流量中捕获的pcap包经初步预处理后形成的csv文件）， 并提取特征字段作为算法输入。

# 输入数据格式
## 参数说明

| 参数              | 说明                          |
|-----------------|-----------------------------|
| --hdfs-host     | HDFS服务器地址，默认为192.168.80.45  |
| --hdfs-port     | HDFS服务端口，默认为8020            |
| --hdfs-username | HDFS用户名                     |
| --hdfs-path     | HDFS服务器内文件地址                |
| --model-local   | 输入文件本地存储路径，默认为根目录           |
| --mysql-host    | mysql数据库地址，默认为192.168.80.45 |
| --mysql-port    | mysql端口号，默认为3306            |
| --mysql-user    | mysql登录用户名                  |
| --mysql-pwd     | mysql登录密码                   |
| --mysql-db      | mysql数据库名称                  |
| --mysql-table   | mysql数据表名称                  |


# 输出结果
输出一个包含特征字段、标签、预测结果的csv文件，保存到mysql数据库中。
