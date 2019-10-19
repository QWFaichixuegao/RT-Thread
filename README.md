# RT-Thread
sugar 精简的RT-Thread使用方法
1、先通过cubemax配置工程 
2、去demo文件夹中拷贝*.yaml配置文件、IDE目录、Src-rtt目录
3、将src目录中的main.c改名为entry.c并复制到Src-rtt目录下覆盖原entry.c
4、git submodule add https://github.com/SuWeipeng/rt-thread.git Libraries/rt-thread将sugar精简的RTT内核作为submodule加入到代码的文件夹下如果刚开始代码未加入smartGit
5、修改entry.c文件包括加入entry.h头文件、修改代码
6、用progen generate -f projects.yaml -p stm32f4discovery-rtt -t uvision5
