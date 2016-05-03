
This repository is deprecated. Due to the way Docker Hub manages automated builds, we've created three repositories which get automatically built. Any future changes will go there.

| GitHub Repository               | Docker Hub Image   |
|---------------------------------|--------------------|
| payara/docker-payaraserver-full | payara/server-full |
| payara/docker-payaraserver-web  | payara/server-web  |
| payara/docker-payaramicro       | payara/micro       |

The latest(default) tag will always contain the most recent release which is currently 161.1 and will shortly be 162. There are also version branches which get built into tags of the same name, e.g:

`docker pull payara/server-full:162`

* Payara is located in the `/opt/payara41` directory. This is deliberately free of any versioning so that any scripts written to work with one version can be seamlessly migrated to the latest docker image.
* Full and Web editions are derived from the OpenJDK 8 images with a Debian Jessie base
* Micro editions are built on OpenJDK 8 images with an Alpine linux base to keep image size as small as possible.
