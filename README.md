
# Overview

This is a project, which contains the automatically generating data transfer objects from the protobuf files.

## Usage

To include the project's classes add the following sections to your project:

```xml
<repositories>
  <repository>
    <id>proto-model-java-mvn-repo</id>
    <url>https://raw.github.com/binary-routing/proto-model-java/mvn-repo/</url>
    <snapshots>
      <enabled>true</enabled>
      <updatePolicy>always</updatePolicy>
    </snapshots>
  </repository>
</repositories>
...
<dependencies>
  ...
  <dependency>
    <groupId>com.xxlabaza.test</groupId>
    <artifactId>proto-model-java</artifactId>
    <version>1.0.1</version>
  </dependency>
  ...
</dependencies>
```

## Deploy

To deploy a new project's version in Github, use the following command:

```bash
$> ./mvnw -s settings.xml clean deploy
```

Where `settings.xml` contains your credentials for Github (with **github** id).
