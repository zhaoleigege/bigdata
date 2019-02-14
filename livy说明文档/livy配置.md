# livy配置

```shell
# 1、前往官网下载livy压缩包
https://livy.incubator.apache.org/download/

# 2、确保系统环境变量设置了SPARK_HOME
SPARK_HOME="/home/zhaolei/Documents/spark"

# 3、进入livy文件夹，创建logs文件夹
mkdir logs

# 3、进入conf文件夹，配置日志文件
cp log4j.properties.template log4j.properties

# 4、配置livy.conf文件
cp livy.conf.template livy.conf
vi livy.conf
# 修改如下内容
livy.spark.master = local							 # spark启动模式为本地模式
livy.file.local-dir-whitelist=/home/zhaolei/Desktop  # jar文件所在的本地目录
```

