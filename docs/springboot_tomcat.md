# springboot 打包使用tomcat运行

> 1.将maven打包方式改为war

![image-20220312155716472](./_media/image-20220312155716472.png)

> 2.将springboot的tomcat依赖的scope改为provided

![image-20220312155844195](./_media/image-20220312155844195.png)

> 3.springboot启动类继承SpringBootServletInitializer

![image-20220312160112375](./_media/image-20220312160112375.png)

> 4.修改application.xml

![image-20220312161024615](./_media/image-20220312161024615.png)

> 5.maven打包

![image-20220312160216204](./_media/image-20220312160216204.png)

> 6.上传到tomcat安装目录下的webapps文件夹

![image-20220312160423010](./_media/image-20220312160423010.png)

如果没有修改context-path的值，可以将war包命名为ROOT，这样不用在路径前加context-path。

ps:可以把原先在webapps里面的文件给删了。

> 7.启动tomcat