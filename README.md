# save_repository
save some files

# use


### normal
```
https://raw.githubusercontent.com/sltpaya/save_repository/master/install1.gradle
https://raw.githubusercontent.com/sltpaya/save_repository/master/upload1.gradle
```

### with gpg
```
https://raw.githubusercontent.com/sltpaya/save_repository/master/install1.gradle
https://raw.githubusercontent.com/sltpaya/save_repository/master/upload2.gradle
```


### problem

* encoding
```
tasks.withType(JavaCompile) {
    options.encoding = "UTF-8"
}
```
* javadoc error and encoding
```
javadoc {
    failOnError false
    options {
        encoding "UTF-8"
        charSet 'UTF-8'
        author true
        version true
    }
}
```

### module gradle

```
ext {
    bintrayName = 'your artifact name'
    artifact = bintrayName
    libraryName = 'library name like 'Web Intercept annotation''
    libraryDescription = 'The annotation used in Web Intercept'
    libraryVersion = "1.0"
}
```

### gradle.properties

```
bintrayRepo=maven
publishedGroupId=com.sltpaya.open
siteUrl=https://github.com/sltpaya
gitUrl=https://github.com/sltpaya
developerId=sltpaya
developerName=sltpaya
developerEmail=sltpaya@163.com

licenseName=The Apache Software License, Version 2.0
licenseUrl=http://www.apache.org/licenses/LICENSE-2.0.txt
allLicenses=["Apache-2.0"]
```

### local.properties

```
bintray.user=******
bintray.apikey=******

```
