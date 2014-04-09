HOWTO build Hadoop Native Libs
------------------------------
+ Install packages for Hadoop build: *jdk >= 6*, *maven*, *cmake*, *protobuf >= 2.5.0*
+ Get Hadoop source code:
```bash
$ wget http://archive.apache.org/dist/hadoop/core/hadoop-2.3.0/hadoop-2.3.0-src.tar.gz
```
+ Unpack source
```bash
$ tar xvf hadoop-2.3.0-src.tar.gz
```
+ Build Hadoop
```bash
$ cd hadoop-2.3.0-src
$ mvn package -Pdist,native -DskipTests -Dtar
```
+ Create tarball with Hadoop Native Libs
```bash
$ cd /hadoop-dist/target/hadoop-2.3.0/lib
$ tar -czvf hadoop-native-libs-2.3.0.tar.gz native
```
