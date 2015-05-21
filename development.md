

# IDE Configuration #
There are many ways to develop applications in android i will describe here how my enviroment is set up .

# Software requirements #
first of all i am using Ubuntu as my primary operating system it is not required to develop but i won't be
going in to details how to make it work on windows. There are some shell scripts and they will work in linux
environment (not many mostly in graphics) and also some parts will be written in c.

  1. Eclipse -  can be downloaded here : http://www.eclipse.org/ i use ide for EE
  1. Android SDK - http://developer.android.com/sdk/index.html i won't be writing how to set it all up there is plenty of documentation in the internet
  1. Mercurial eclipse - http://www.vectrace.com/mercurialeclipse/ again install plugin in eclipse


# how to compile  Android App #
  1. clone two projects from the repository [common](https://code.google.com/p/valkyrie-android/source/browse?repo=valkyrie-common) and [valkyrie-apk](https://code.google.com/p/valkyrie-android/source/browse?repo=valkyrie-apk)

> using commandline in your source dir:
```
  hg clone https://valkyrie-apk.valkyrie-android.googlecode.com/hg/ valkyrie-android-valkyrie-apk 
  hg clone https://valkyrie-common.valkyrie-android.googlecode.com/hg/ valkyrie-android-valkyrie-common
```
> or using mercurial eclipse

  1. create  and start android runtime or connect your phone
  1. right click on valkyrie-apk and run as android application

after that application should start and should be able to log in to the Dev Server.


# how to compile server #
NOT READY YET
just some random commands
```
mvn -Prun-server clean compile jar:jar  sgs:install sgs:configure sgs:deploy sgs:deploy-dependencies sgs:boot
```