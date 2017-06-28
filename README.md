# liblucene2-java-maven Debian package

Official `liblucen2-java` Debian package installs .jars only into `/usr/share/java`, but not into local Maven repo (`/usr/share/maven-repo`)

The current package simply depends on `liblucene2-java` and creates necessary symlinks and POM files in Debian local Maven repo, so that `org.apache.lucene:lucene-core:2.x` and other artifact are available from that repo.

The version is indicated as `2.9.x` in the Maven repo to avoid conflicts with other `libluceneX-java` packages.

Be careful: generated POM files don't include any dependencies at the moment. Will be fixed if necessary.

