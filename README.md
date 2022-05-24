# maven

2 adet uygulama aşağıda görüldüğü gibi fark yoktur. Ancak -DarchetypeArtifactId=maven-archetype-quickstart ile jakartaEE uygulama create ederseniz faklı olacaktır. 

link: https://www.tutorialspoint.com/maven/maven_quick_guide.htm


![image](https://user-images.githubusercontent.com/9527118/169993701-9819c379-c25f-45a5-aab7-c15a75fe2869.png)

![image](https://user-images.githubusercontent.com/9527118/169993325-945049d1-ea97-4e01-bf99-78c8a049e79d.png)


```

mvn archetype:generate -DgroupId=com.ornek.maven -DartifactId=basit1 -DinteractiveMode=false
mvn archetype:generate -DgroupId=com.ornek.maven -DartifactId=basit2 -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false

$ diff basit1 basit2/
diff basit1/pom.xml basit2/pom.xml
5c5
<   <artifactId>basit1</artifactId>
---
>   <artifactId>basit2</artifactId>
8c8
<   <name>basit1</name>
---
>   <name>basit2</name>
Common subdirectories: basit1/src and basit2/src

```


# mvn site

hazırlamış olununa proje ile ilgili bir html web sitesi oluştururu :-

$ ls -alh
total 68K
drwxrwxr-x 4 kullan kullan 4.0K May 24 12:05 .
drwxrwxr-x 6 kullan kullan 4.0K May 24 12:05 ..
drwxrwxr-x 2 kullan kullan 4.0K May 24 12:05 css
-rw-rw-r-- 1 kullan kullan 8.8K May 24 12:05 dependencies.html
-rw-rw-r-- 1 kullan kullan 4.4K May 24 12:05 dependency-info.html
drwxrwxr-x 3 kullan kullan 4.0K May 24 12:05 images
-rw-rw-r-- 1 kullan kullan 2.8K May 24 12:05 index.html
-rw-rw-r-- 1 kullan kullan 5.3K May 24 12:05 plugin-management.html
-rw-rw-r-- 1 kullan kullan 4.8K May 24 12:05 plugins.html
-rw-rw-r-- 1 kullan kullan 4.1K May 24 12:05 project-info.html
-rw-rw-r-- 1 kullan kullan 3.9K May 24 12:05 summary.html

![image](https://user-images.githubusercontent.com/9527118/169994889-271291d6-bd5e-4fae-8966-4528e2424330.png)

