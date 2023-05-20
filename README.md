# MIT_2020_6.s081
本仓库记录实现整个课程lab的全过程



# 0 环境配置

1. docker 配置环境
本人直接是使用的docker进行环境配置，使用`Vscode`进行远程连接编码，开盖即用，很方便。
```
docker pull linxi177229/mit6.s081
docker run -t -i --name mit6.s081 linxi177229/mit6.s081 /bin/bash
// 之后启动容器使用
docker start mit6.s081
docker attach mit6.s081
```

2. 具体测试
编码完成之后在`makefile`的`UPROGS`中加入编码完成的文件名，使用`make qemu` 重新编译。
自带一个测试程序，如可以使用命令 `./grade-lab-util sleep` 测试 第一个实验的sleep实现；

# 1 utilities
这个是第一个lab，主要是熟悉xv6、lab实验如何做等。

其中有一个并行化素数筛可以参考实验hint中提到的那篇文章，[Bell Labs and CSP Threads](https://swtch.com/~rsc/thread/)
下面这张图对理解这个筛法很有帮助
![并行化素数筛](https://swtch.com/~rsc/thread/sieve.gif)






