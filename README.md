AOSP+RRO MarshMallow
===========

To initialize your local repository using the AOSP-RRO trees, use a command like this:
````bash
repo init -u git://github.com/AOSP-RRO/manifest.git -b M-6.0
```
Add Onyx resources by typing this:
````bash
curl --create-dirs -L -o .repo/local_manifests/onyx.xml -O -L https://raw.githubusercontent.com/L-Aosp/manifest/default/onyx.xml
```
Then to sync up:
````bash
repo sync
```
Finally to build:
````bash
./build.sh device_codename
```
Example:
````bash
./build.sh falcon
./build.sh titan
```
