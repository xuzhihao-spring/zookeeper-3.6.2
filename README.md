1. 下载地址
	https://github.com/apache/zookeeper/tree/release-3.6.2

2. 准备配置文件
	1. 复制zoo_sample.cfg更名为zoo.cfg,修改dataDir
	2. 将conf下的log4j.peoperties复制到zookeeper-server的resources下
	3. 在zookeeper-server下src/main/resource上，鼠标右键，Mark Directory as -> Root Resources

3. 启动异常
	1. 程序包org.apache.zookeeper.data不存在 root项目compile
	2. NoClassDefFoundError: com/codahale/metrics/Reservoir provided去掉
