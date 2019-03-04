pom.xml:
```xml
    <repositories>
        <repository>
            <id>my-maven-repo</id>
            <url>https://raw.githubusercontent.com/wengsongwei8/maven-repo/master</url>
        </repository>
    </repositories>
```

使用方法：
源项目中使用：
```xml
    <distributionManagement>
        <repository>
            <id>local-maven</id>
            <url>file:D:/mywork/maven-repo</url>
        </repository>
    </distributionManagement>
```

先使用deploy命令，发布到本地：D:/mywork/maven-repo

然后使用以下命令提交：
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/wengsongwei8/maven-repo.git
git push -u origin master
