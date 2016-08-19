This is a Maven repository with containing some unofficial builds of
some software.

Add to the ```pom.xml```:

```
<repositories>
    ...
    <repository>
        <id>sba1-mvn-repo</id>
        <url>https://raw.githubusercontent.com/sba1/mvn-repo/master/</url>
        <snapshots>
            <enabled>true</enabled>
            <updatePolicy>always</updatePolicy>
        </snapshots>
    </repository>
    ...
</repositories>
```
== TeaVM ==

```
$ mvn deploy -DaltDeploymentRepository=sonatype-nexus-snapshots::default::file://REPO_FULL_PATH -DskipTests
```
