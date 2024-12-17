# 介绍

本项目代码原用于，将更纱黑体的信息改为微软雅黑和宋体的，来替换 Windows 系统的默认字体。

现在改为，通过更纱黑体的源码，将思源黑体和 Segoe UI 结合为微软雅黑和宋体。

该字体主要是使用了更纱黑体的 Hint 机制，能够提供更锐利的显示效果。

# 构建流程

1. 参考原版微软雅黑，移除 Segoe UI 中大多数 OpenType 特性；

2. 将 Segoe UI 伪装成 Inter 字体，替换更纱黑体项目的源字体；

3. 修改更纱黑体源码，保留 Segoe UI 中的 Hinting；

4. 执行更纱黑体的构建流程，得到构建出的更纱黑体；

5. 修改更纱黑体字体信息，伪装成微软雅黑和宋体。

# 接下来

1. 编写更加自动化的代码，而不是靠手搓；

2. 能够实现输入任意中文字体和拉丁字体，构建出包含 Hinting 的合成字体。