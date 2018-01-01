1. repo 初始化（如何获取 repo 命令，自行 google）：
```shell
repo init -u https://github.com/liangzhitao/repo-manifest.git -b default
```
2. 同步代码：
```shell
repo sync -j8
```
3. 所有子项目都切到 master 分支：
```shell
#repo forall -c 'git checkout master'
repo start --all master
```
4. 代码全部 clone 下来后，将 projects 目录导入 Android Studio；
5. 在根目录下执行 `gradle clean install`；
6. 打开根目录下的 default.xml，默认所有模块都是放开注释的，需要开发哪个模块，将其他模块注释掉即可。
