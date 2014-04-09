HOWTO build Hadoop Native Libs
==============================
1. Install packages for Hadoop build: *jdk>=6*, *maven*, *cmake*, *protobuf>=2.5.0*
2. Get Hadoop source code
  ```bash
$ wget http://archive.apache.org/dist/hadoop/core/hadoop-2.3.0/hadoop-2.3.0-src.tar.gz
  ```
3. Unpack archive
  ```bash
$ tar xvf hadoop-2.3.0-src.tar.gz
  ```bash
4. Build Hadoop
  ```bash
$ cd hadoop-2.3.0-src
$ mvn package -Pdist,native -DskipTests -Dtar
  ```
