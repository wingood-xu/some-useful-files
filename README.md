# some-useful-files

1. mongoDB配置启动项,可以参考的[博客](https://www.cnblogs.com/lecaf/archive/2013/08/23/mongodb.html):

2. mod_wsgi替换.so文件(查看好多资料有提到导入.so文件,后来发现最近的版本不好使,但是此方法可以解决).

3. SSR app.

4. 本机为部署scrapyd于 2017/11/21 修改D:\Anaconda3\Lib\site-packages\automat\\_methodical.py 文件
      - 修改内容如下:
      
```python
    # 两处修改
    @attr.s(frozen=true)==>@attr.s()
```
5.pip更新所有包命令：pip freeze --local | grep -v '^\-e' | cut -d = -f 1  | xargs pip install -U
