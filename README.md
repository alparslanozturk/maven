# maven

## basit-uygulama

2 adet uygulama aşağıda görüldüğü gibi fark yoktur. Ancak -DarchetypeArtifactId=maven-archetype-quickstart ile jakartaEE uygulama create ederseniz faklı olacaktır. 

![image](https://user-images.githubusercontent.com/9527118/169993484-0787ec31-ab5d-44e0-b1e4-d1e01d3c3faa.png)

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


