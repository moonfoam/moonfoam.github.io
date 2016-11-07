# 2016-11-7
- 现象:Hexo 本地预览没问题，deploy后主页显示大面积空 - theme Next
- 解决方案: <https://github.com/iissnan/hexo-theme-next/issues/1214>

```
iissnan:
不清楚为什么 GitHub Pages 过滤掉了 source/vendors 目录的访问。我提交了一个更新到 master 分支上，修正这个问题，可以更新下。
也可以手动将 source/vendors 目录修改成 source/lib （或者其他的名称，只是 lib 我测试了可以使用）；同时，修改下主题配置文件_config.yml， 将 _internal: vendors 改成你所修改的名字，例如 _internal: lib。
```
