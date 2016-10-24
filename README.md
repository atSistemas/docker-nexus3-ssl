# sonatype/docker-nexus3

A Dockerfile for Sonatype Nexus Repository Manager 3.0.2 with ssl support, based on sonatype/docker-nexus3 image (tag 3.0.2).

All options are the same an are explained in https://github.com/sonatype/docker-nexus3/blob/3.0.2/README.md

This image add support for ssl and new variables/options are described below.


- By default the Dockerfile creates a keystore directory `/nexus-keystore` and a `keystore.jks` in. The passwords for the keystore are `changeit`

- If you want to use your own keystore, create one with the name `keystore.jks`, mount the volume in /nexus-keystore and pass these variables to the docker:

* `KEYSTOREPASSWORD`. Defaults to changeit

* `KEYMANAGERPASSWORD`. Defaults to changeit

* `TRUSTSTOREPASSWORD`. Defaults to changeit
