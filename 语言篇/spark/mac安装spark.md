# 1 安装-mac



**安装准备**

(1) 安装jdk8

官网下载， 这个好像比较慢https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html


我把下载好的放到了百度网盘上: https://pan.baidu.com/s/1fpiSse78YObfalSerql4Zw 提取码: t6q3

```
vim ~/.bash_profile
## 添加如下环境变量信息
export JAVA_HOME="/Library/Java/JavaVirtualMachines/jdk1.8.0_191.jdk/Contents/Home/"
export PATH="$JAVA_HOME/bin:$PATH"
```

(2) 官网下载 http://mirror.bit.edu.cn/apache/spark/spark-2.4.0/spark-2.4.0-bin-hadoop2.7.tgz
或者 `brew install apache-spark`

然后将文件解压到想要放到的目录，我这里是/Users/zhengzhenzhen/ 为例方便版本管理以及后续使用，可以创建一个软链

```
ln -s /Users/zhengzhenzhen/spark-2.4.0-bin-hadoop2.7 /Users/zhengzhenzhen/spark
```

（3） 

```
pip install pyspark
```




**使用jupyter nootbook**

在jupyter notebook中使用pyspark，需要配置环境变量

```
# 基于python的版本
export PYSPARK_DRIVER_PYTHON=jupyter
export PYSPARK_DRIVER_PYTHON_OPTS='notebook'
```



## 参考资料

https://www.jianshu.com/p/f284b77289ca

https://www.jianshu.com/p/cc83d047383d

