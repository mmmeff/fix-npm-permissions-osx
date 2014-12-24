fix-npm-permissions-osx
=======================

This is a scattergun fix for permissions issues (needing sudo for npm install -g) on OSX

Just run the following commands and you should be set. And don't do this on a shared machine,
especially if you share it with other developers (there's got to be one of you out there).

```
sudo chown -R `whoami` ~/.npm
sudo chown -R `whoami` /usr/local/bin/npm
sudo chown -R `whoami` /usr/local/lib/node_modules
```
