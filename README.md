[ProjectGithubUrl]: https://github.com/spoqa/LongPressListener
[PlatformBadge]: https://img.shields.io/badge/Platform-Android-blue.svg
[LicenceUrl]: https://opensource.org/licenses/MIT
[LicenseBadge]: https://img.shields.io/badge/License-MIT-blue.svg
[BintrayUrl]: https://android-arsenal.com/details/1/7134
[BintrayBadge]: https://img.shields.io/bintray/dt/spoqa/maven/LongPressListener.svg

# LongPressListener

[![Platform][PlatformBadge]][ProjectGithubUrl]
[![License][LicenseBadge]][LicenceUrl]
[![BintrayBadge]][BintrayUrl]
---------

Android long press(click) listener with custom duration ✨

## ScreenShot
TBD

## Setup
Install library with Gradle

### Gradle:
Add this to your project level build.gradle:

```groovy
buildscript {
    repositories {
        jcenter()
    }
}
```

Add this to your app build.gradle:

```groovy
dependencies {
    implementation "com.spoqa.longpresslistener:LongPressListener:1.0.0"
}
```

## Usages
```kotlin
view.setOnTouchListener(OnLongPressListener(
    object : OnLongPressCallback {
        override fun onPress() {
            // Your action after long press
        }
    ),
    duration = 3000L  // Optional
))
```

### With Kotlin Extensions
```kotlin
view.onPress({
    // Your action after long press
})
```


## License
 ```
Copyright 2020 Spoqa


Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

```
