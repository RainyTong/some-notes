# MaxOS: python2 python3 pip pip3傻傻分不清楚

- **事情起因**：

用 `pip install --ignore-installed --upgrade tensorflow -i https://pypi.doubanio.com/simple/` 这段命令更新tensorflow明明显示更新成功，但是
python3里面对应的tensorflow还是老版本

- **发现问题**：

In my Macbook Pro, there is a default python2 in the path: `/usr/local/lib/python2.7`.

There is also a installed python3 in the path: `/Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6`.

So when I use `pip` to install tensorflow, it will be installed in `/usr/local/lib/python2.7/site-packages`.

- **解决问题**：

Use `python3 -m pip install --ignore-installed --upgrade tensorflow -i https://pypi.doubanio.com/simple/` to install/update tensorflow, tf will 
be installed in `/Library/Frameworks/Python.framework/Versions/3.6/lib/python3.6/site-packages`.

*Please remember to use `python3 -m pip install` to replace `pip3 install`!!!* :pray::pray::pray:
