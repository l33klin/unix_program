# unix_program
鉴于是练习，代码逻辑很简单，所以先采用gcc编译

### APUE 练习代码
**IDE:** JetBrains CLion 2019.1

**运行机器:** MacBook Pro (Retina, 15-inch, Mid 2015) &&

**编译工具:** cmake

### 编译&运行方法
1. 编译apue依赖库:
```bash
$ cd include    # 切换到include目录
$ gcc -o apue.o -c apue.cpp
```
2. 编译自己的代码，这里比如我们想编译`Chapter1/1-1_ls1.cpp`:
```bash
$ cd Chapter1
$ gcc -o ls1 1-1_ls1.cpp -L ../include/ -l apue.o
```
3. 得到`ls.o`文件，即可运行
```bash
$ ./ls1.o .
.
..
CMakeLists.txt
ls1.o
1-2_cp1.cpp
1-1_ls1.cpp
```


### 参考:
1. cmake介绍：https://www.hahack.com/codes/cmake/