HOWTO build Hadoop Native Libs
==============================
+ Install packages for Hadoop build: *jdk>=6*, *maven*, *cmake*, *protobuf>=2.5.0*
+ Get Hadoop source code:
```bash
$ wget http://archive.apache.org/dist/hadoop/core/hadoop-2.3.0/hadoop-2.3.0-src.tar.gz
```
+ Unpack archive
```bash
    $ tar xvf hadoop-2.3.0-src.tar.gz
```
+ Build Hadoop
```
$ cd hadoop-2.3.0-src
$ mvn package -Pdist,native -DskipTests -Dtar
```
