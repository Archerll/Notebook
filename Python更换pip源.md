# Python更换pip源

## 几个国内常用的镜像

阿里云 [http://mirrors.aliyun.com/pypi/simple/](https://links.jianshu.com/go?to=http%3A%2F%2Fmirrors.aliyun.com%2Fpypi%2Fsimple%2F)
中国科技大学 [https://pypi.mirrors.ustc.edu.cn/simple/](https://links.jianshu.com/go?to=https%3A%2F%2Fpypi.mirrors.ustc.edu.cn%2Fsimple%2F)
豆瓣 [http://pypi.douban.com/simple/](https://links.jianshu.com/go?to=http%3A%2F%2Fpypi.douban.com%2Fsimple%2F)
清华大学 [https://pypi.tuna.tsinghua.edu.cn/simple/](https://links.jianshu.com/go?to=https%3A%2F%2Fpypi.tuna.tsinghua.edu.cn%2Fsimple%2F)
中国科学技术大学 [http://pypi.mirrors.ustc.edu.cn/simple/](https://links.jianshu.com/go?to=http%3A%2F%2Fpypi.mirrors.ustc.edu.cn%2Fsimple%2F)

## 临时更换pip源

例如使用 阿里镜像下载numpy

```shell
pip install numpy -i http://mirrors.aliyun.com/pypi/simple/
```



## 永久更换pip源

如果想要一劳永逸，那可以尝试永久更换pip源

Windows环境

```shell
pip config set global.index-url='http://mirrors.aliyun.com/pypi/simple/'
```



