# tinyrenderer

## 仓库的作用

作为学习GitHub开源项目：
[tinyrenderer](https://github.com/ssloy/tinyrenderer) 的过程记录，可通过commit记录查看不同的快照。

## 如何编译并运行本项目

首先克隆本项目到本地：
```bash
git clone https://github.com/sprout-37/tinyrenderer.git
```

然后进入文件夹：

```cmake
cd tinyrenderer
```

通过cmake进行配置与编译：
```cmake
cmake -B build
cmkae --build build
```

运行可执行文件：
```cmake
./build/tinyrenderer/tinyrenderer
```

可看到结果文件`output.tga`。
