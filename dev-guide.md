# Lanxi Standard Development

### 常量
  - 公司GIT地址：git@192.168.17.180:/data/git/项目名.git
  - JAVA WEB 通用模板地址：git@192.168.17.180:/data/git/template.git
  - 公司FTP地址：



### 工具
- Git: [Git简易指南][git]
    - add
    - commit
    - pull
    - push
    - log
    - status
    - reset
    - revert
    - branch
    - checkout
    - merge
    
    
- IDEA: [IDEA官方入门指南][idea]

- Maven:
  - [Maven入门][maven]
  - 添加阿里云镜像，cp <maven_path>/conf/setting.xml ~/.m2/ 并将以下代码加入文件的
  `<mirrors></mirrors>`标签之间

        <mirror>
          <id>alimaven</id>
          <name>aliyun maven</name>
          <url>http://maven.aliyun.com/nexus/content/groups/public/</url>
          <mirrorOf>central</mirrorOf>
        </mirror>




- Markdown: [Markdown语法手册][markdown]

- Atom:[Atom下载][atom]

### 1.前端
- [HTML和CSS编写规范](http://codeguide.bootcss.com/)
- 页面通用模块抽出，方便后续维护

index.jsp
 ``` html
    <%@ page contentType="text/html;charset=UTF-8" language="java" %>
    <html>
    <head>
      <title>INDEX</title>
      <!--
          导入通用页面
          <%@ include file="filename"%>
      -->
      <%@ include file="common.jsp"%>
    </head>
    <body>

    </body>
    </html>
  ```

  common.jsp
  ``` html
  <%@ page contentType="text/html;charset=UTF-8" language="java" %>
  <script type="text/javascript">
      alert('通用页面');
  </script>
  ```


### 2.后台




### 3.交互
1. 命名规范

2. 调用规范
3.



### 4.数据库

  +------+-------+
  |表|t_example|
  |视图|t_example|
  |存储过程|t_example|
  +------+-------+

[TOC]

``` python
@requires_authorization
def somefunc(param1='', param2=0):
    '''A docstring'''
    if param1 > param2: # interesting
        print 'Greater'
    return (param2 - param1 + 1) or None
class SomeClass:
    pass
>>> message = '''interpreter
... prompt'''
```



[git]: http://www.bootcss.com/p/git-guide/  "git指南"
[idea]: http://www.jianshu.com/p/24efaf33dcd3 "idea指南"
[maven]: http://www.jianshu.com/p/ede040d8ab0f "maven指南"
[markdown]: http://www.jianshu.com/p/fdb5cbdaf244 "markdown指南"
[atom]: https://atom.io/ "atom下载"
