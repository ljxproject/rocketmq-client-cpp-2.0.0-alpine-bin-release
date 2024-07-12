# rocketmq-client-cpp-2.0.0-alpine-bin-release



## 使用方式

步骤一：先在docker镜像构建机上解压

步骤二：在dockerfile文件下添加下面命令

```
ADD --chmod=755 ./rocketmq-client-cpp-2.0.0-alpine-bin-release ./rocketmq-client-cpp
RUN ln -s {Absolute path}/rocketmq-client-cpp/bin/librocketmq.so /usr/lib/librocketmq.so
RUN ldconfig /usr/lib
```

