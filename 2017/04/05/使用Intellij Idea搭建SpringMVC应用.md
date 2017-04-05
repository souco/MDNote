#### 使用 Intellij Idea 搭建 web 应用

期间，报错`NoClassDefFoundError: javax/servlet/jsp/jstl/core/Config`，应该是由缺少`standard.jar`和`jstl.jar`的 jar 包引起的。

在`http://archive.apache.org/dist/jakarta/taglibs/standard/binaries/`下载jar包，放入lib目录下，此时报错。 `el-api-2.2.jar`和 tomcat 提供的包冲突了,删掉`el-api-2.2.jar`，重启tomcat，正常。
