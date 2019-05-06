# maven功能
* 将两个web工程合并打包（maven-demo-web合并到maven-demo-job中）
* 打包时指定web.xml(<webXml>src/main/webapp/WEB-INF/jboss-web.xml</webXml>)
* 打包时拷贝代码中的xml文件到对应目录(maven-resources-plugin)
* 打ear包

#  参考文档
* https://rsy.iteye.com/blog/2296802

# 将两个web工程合并打包（maven-demo-web合并到maven-demo-job中）
* maven-demo-job在相同位置已经存在的文件会覆盖maven-demo-web中的文件
* 可以指定maven-demo-web通过class的文件合并，也可以使用jar的形式（没试验）
* maven-demo-web打war时要指定<attachClasses>true</attachClasses>
* maven-war-plugin

# 打ear包
* jboss-deployment-structure.xml是为jboss准备的