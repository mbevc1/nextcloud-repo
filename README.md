[![Pipeline](https://github.com/mbevc1/nextcloud-repo/actions/workflows/build.yml/badge.svg)](https://github.com/mbevc1/nextcloud-repo/actions/workflows/build.yml)
[![pages-build-deployment](https://github.com/mbevc1/nextcloud-repo/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/mbevc1/nextcloud-repo/actions/workflows/pages/pages-build-deployment)

# nextcloud-repo
Nextcloud RPM repo

## RHEL/CentOS

Add repository setting:

```
$ sudo vim /etc/yum.repos.d/nextcloud.repo
[nextcloud]
name=Nextcloud repository
baseurl=http://nc.bevc.net/releases/$releasever/$basearch/
gpgcheck=0
enabled=1
$ sudo yum -y update
$ sudo yum -y install nextcloud
```
