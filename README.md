## Logback BOM
Bill of materials for Logback.

## Usage
In your parent POM or project POM, add the BOM to the `dependencyManagement` section:
```
<dependencyManagement>
    <dependencies>
        ...
        <dependency>
            <groupId>com.eoniantech.build</groupId>
            <artifactId>logback-bom</artifactId>
            <version>1.3.0-alpha4</version>
            <type>pom</type>
            <scope>import</scope>
        </dependency> 
        ...
    </dependencies> 
<dependencyManagement>
```

Then, in the `dependencies` section of your project POM, depend on specific Logback components without the version:

```
<dependencies>
    ....
    <dependency>
        <groupId>ch.qos.logback</groupId>
        <artifactId>logback-classic</artifactId>
        <scope>runtime</scope>
    </dependency>
    ...
</dependencies>   
