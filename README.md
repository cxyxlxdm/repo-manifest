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
