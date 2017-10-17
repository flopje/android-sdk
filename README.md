# Android SDK for Docker [![](https://images.microbadger.com/badges/image/flopje/android-sdk.svg)](https://microbadger.com/images/flopje/android-sdk)

This image contains the latest versions of Android SDK and Gradle. Feel free to contribute ;)

## Examples

### Start a container and open the shell

```
docker run -it flopje/android-sdk bash
```

### Build the project in current directory

```
docker run -it -v $(pwd):/home/user/project -w /home/user/project -u $(id -u):$(id -g) flopje/android-sdk gradle build
```

### Persistent Android SDK and caches

* `-v android-sdk:/home/user/android-sdk-linux`
* `-v gradle-cache:/home/user/.gradle`
* `-v android-cache:/home/user/.android`
