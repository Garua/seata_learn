####说明
- config.txt是上传到nacos配置中心配置文件(已做过修改)，
- file.conf,register.conf是seata服务端的配置文件

#### 把相关配置上传到nacos配置中心
[上传脚本](https://github.com/seata/seata/blob/develop/script/config-center/nacos/nacos-config.sh)

`上传命令` 
```
sh ${SEATAPATH}/script/config-center/nacos/nacos-config.sh -h localhost -p 8848 -g SEATA_GROUP -t 5a3c7d6c-f497-4d68-a71a-2e5e3340b3ca -u username -w password
```

[seata官方配置文件样例](https://github.com/seata/seata/blob/develop/script/config-center/config.txt)
#### 通常我们只需要修改样例配置文件中的数据库信息和事务分组名