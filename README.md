# pqi: a terminal tools for Python ![MIT License][license-badge]

由于国内通过pip下载python包的速度真的很慢，而pqi可以把PyPi源迅速切换化为国内源tuna, douban, aliyun, ustc从而加快python包的安装速度。

```
             _ __      _,.---._      .=-.-.
          .-`.' ,`.  ,-.' - ,  `.   /==/_ /
         /==/, -   \/==/ ,    -  \ |==|, |  
        |==| _ .=. |==| - .=.  ,  ||==|  |  
        |==| , '=',|==|  : ;=:  - ||==|- |  
        |==|-  '..'|==|,  '='  ,  ||==| ,|  
        |==|,  |    \==\ _   -    ;|==|- |  
        /==/ - |     '.='.  ,  ; -\/==/. /  
        `--`---'       `--`--'' `--`--`-`   

                        ---- by Hangfeng Yang

```

## 怎么使用(兼容py2/py3/linux/windows/MacOS)
### 1.安装
#### 方法一（推荐）
```
>>> pip install pqi
```

#### 方法二
```
>>> git clone https://github.com/Fenghuapiao/PyQuickInstall.git
>>> python3 setup.py install
```


### 2. 命令行输入 `pqi` 回车
```
>>> pqi
Usage:
  pqi ls
  pqi use <name>
  pqi show
  pqi add <name> <url>
  pqi remove <name>
  pqi (-h | --help)
  pqi (-v | --version)
Options:
  -h --help        Show this screen.
  -v --version     Show version.
```
* 列举所有支持的PyPi源
```
>>> pqi ls
```

* 改变PyPi源
```
>>> pqi use <name>
```
例子，比如运行`pqi use tuna`即把当前PyPi源改为清华的PyPi源

* 显示当前PyPi源
```
>>> pqi show
```

* 添加新的pip源(如添加USTC源）
```
>>> pqi add ustc https://mirrors.ustc.edu.cn/pypi/web/simple
```

* 移除pip源（如官方PyPi源）
```
>>> pqi remove pypi
```

### 3. 升级到最新版`pqi`
```
>>> pip install --upgrade pqi
```

## LICENSE
[MIT](https://github.com/Fenghuapiao/PyQuickInstall/blob/master/LICENSE)

[license-badge]:   https://img.shields.io/badge/license-MIT-007EC7.svg
