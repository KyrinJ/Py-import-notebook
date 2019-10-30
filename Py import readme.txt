#1 
bs4文件夹复制到 Lib/site-packages
Tools/scripts/2to3.py 复制到 Lib
cmd:  cd: Lib>pyhon 2to3.py bs4 -w
cmd:  cd: bs4文件夹>python setup.py install
                   >python
>>> from bs4 import BeautifulSoup
>>> import bs4

#2
cmd:  cd: requests文件夹>python setup.py install
                        >python
>>> import requests

#3
import pip
print(pip.pep425tags.get_supported())
→www.lfd.uci.edu/~gohlke/pythonlibs/#lxml
cmd:
遇到ascii编码问题。site-packages下加 sitecustomze.py 再升级 pip 至18.0
>python -m pip install lxml