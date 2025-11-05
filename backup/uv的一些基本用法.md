为了解决项目之间的依赖冲突，使用以下命令创建虚拟环境：

```
python -m venv .venv
```

但 uv 更方便，只需这样就能初始化：

```
uv init
```

使用 pyproject.toml 文件来管理配置文件。


```
name = "my_project"
version = "1.0.0"
requires-python = ">=3.9,<3.13"
dependencies = [
  "astropy>=5.0.0",
  "pandas>=1.0.0,<2.0",
]
```


uv 封装了一些底层命令。 

添加包的时候

```
uv add flask
```

这会将依赖加入到 pyproject.toml 文件并创建虚拟环境。

使用别人的项目时，使用

```
uv sync
```

运行代码时。

首先需要激活环境（在 IDE 中无需此步骤）：

```
source .venv/bin/activate
```

再运行：

```
python main.py
```

uv 也提供了一个更加直接的做法：

```
uv run main.py
```

这无需手动激活环境。

## 参考资料

1. 程序员老王的视频：[从pip到uv：一口气梳理现代Python项目管理全流程！](https://youtu.be/jd1aRE5pJWc?si=YV3K1wrSGZ3oVeXa)
2. [十年来Python生态最好工具，引爆全社区的uv到底是什么？](https://mp.weixin.qq.com/s/f3KpA2lYPqI2BM86dMfETA)
3. [uv is the best thing to happen to the Python ecosystem in a decade - Blog - Dr. Emily L. Hunt](https://emily.space/posts/251023-uv)
