## tomcat 9.0.x 学习笔记

学习课程对应 https://www.bilibili.com/video/BV1rY411m7Sw

- 编译完成之后，java 目录下 `javax` 主要定义规范，`org.apache` 主要负责实现。
- 可以选择创建 home 目录，使得调试文件目录结构更清晰
- 设置 tomcat 启动参数
```bash
# JVM参数 注意path替换
-Dcatalina.home=C:\Users\Administrator\Documents\tomcat-9.0.x-learning\home
-Dcatalina.base=C:\Users\Administrator\Documents\tomcat-9.0.x-learning\home
-Djava.util.logging.manager=org.apache.juli.ClassLoaderLogManager
-Djava.util.logging.config.file=C:\Users\Administrator\Documents\tomcat-9.0.x-learning\home\conf\logging.properties
-Dfile.encoding=utf-8
# 启动类
org.apache.catalina.startup.Bootstrap
```
- 修改字符解码集、添加 JSP 初始化器
- 可以使用 Enterprise Architect 工具绘制 UML 图
