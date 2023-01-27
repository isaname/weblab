# sphinx

## 使用步骤

>1. 安装`pip install sphinx`
>
>
>2. 快速启动
>
>  ```powershell
>sphinx-quickstart
>  ```
>
>3. 编译
>
>  ```
>make html
>  ```
>
>

## 添加自己的页面

修改index.rst 文件,

```rst
.. toctree::
   :maxdepth: 2
   :caption: Contents:
   
   pages/S

```

source/pages/S.md 就是自己的文件

## 修改主题

主题网站 : https://sphinx-theme.org

按照里面的介绍操作就行

## 支持markdown

sphinx 默认不支持markdown,安装`pip install recommonmark`,修改**conf.py**

`extention=['recomonmark']`

## 启动本地服务

安装`pip install sphinx-autobuild`

启动`sphinx-autobuild source build/html`

可以实现热加载,访问http://127.0.0.1:8000