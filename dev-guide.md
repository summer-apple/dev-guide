# Lanxi Standard Development

### 常量
  - 公司GIT地址：git@192.168.17.180:/data/git/项目名.git
  - JAVA WEB 通用模板地址：git@192.168.17.180:/data/git/template.git
  - 公司FTP地址：
  - 免密登录：ssh-keygen -t rsa 



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

  ``` xml
  <mirror>
    <id>nexus</id>
    <mirrorOf>*</mirrorOf>
    <url>http://192.168.17.180:8081/nexus/content/groups/public</url>
  </mirror>

  ```



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
- 命名规范

- 调用规范




### 4.数据库


|类型|示例名称|
| ------ | -------- |
|表|t_name|
|视图|v_name|
|存储过程|p_name|
|单词字段|name|
|多词字段|user_type|





[git]: http://www.bootcss.com/p/git-guide/  "git指南"
[idea]: http://www.jianshu.com/p/24efaf33dcd3 "idea指南"
[maven]: http://www.jianshu.com/p/ede040d8ab0f "maven指南"
[markdown]: http://www.jianshu.com/p/1e402922ee32 "markdown指南"
[atom]: https://atom.io/ "atom下载"
