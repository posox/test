HOWTO build Hadoop Native Libs

1. Install packages for Hadoop build:
```
oracle jdk >= 6
maven
cmake
protobuf >= 2.5.0
```

2. Get Hadoop source code:
```sh
$ wget http://archive.apache.org/dist/hadoop/core/hadoop-2.3.0/hadoop-2.3.0-src.tar.gz
```

3. Unpack archive
```sh
$ tar xvf hadoop-2.3.0-src.tar.gz
```sh

4. Build Hadoop
```sh
$ cd hadoop-2.3.0-src
$ mvn package -Pdist,native -DskipTests -Dtar
```
