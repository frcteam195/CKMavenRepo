#CKMavenRepo

Publish artifacts to this repo using this command ```mvn install:install-file -DgroupId=com.team195 -DartifactId=CKIllposedOSCLib -Dversion=0.0.1 -Dfile=../CKIllposedOSCLib.jar -Dpackaging=jar -DgeneratePom=true -DlocalRepositoryPath=.  -DcreateChecksum=true```

Use with this configuration:
```repositories {
    mavenCentral()

    maven {
        url "http://raw.github.com/frcteam195/CKMavenRepo/master"
    }
}```

Then inside dependencies
```compile group: 'com.team195', name: 'CKIllposedOSCLib', version: '0.0.1'```
