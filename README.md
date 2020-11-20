# Video Opener Library

[![](https://jitpack.io/v/GalShashua/VideoOpenerLibrary.svg)](https://jitpack.io/#GalShashua/VideoOpenerLibrary)

![screenshot0](https://user-images.githubusercontent.com/56959832/99788323-a2357d00-2b29-11eb-95f2-de9b57415958.JPG)
![screenshot3](https://user-images.githubusercontent.com/56959832/99791789-d1022200-2b2e-11eb-80b5-8d49cf2de8f5.JPG)

A library for open video (mp4) easly.
With options to run the video 10 seconds forward or backward, stop and continue.

## Setup
Step 1. Add it in your root build.gradle at the end of repositories:
```
allprojects {
    repositories {
	    maven { url 'https://jitpack.io' }
    }
}
```

Step 2. Add the dependency:

```
dependencies {
  implementation 'com.github.GalShashua:VideoOpenerLibrary:1.00.01'
}

```

## Usage
```java

// For continual calls - 
VideoLibrary.openVideo(MainActivity.this, 
		"https://i.imgur.com/czpUGYA.mp4");
		
more videos example : https://i.imgur.com/x3Ykda2.mp4
		      https://i.imgur.com/AYgFAOl.mp4
	
```	


## License
```	

    Copyright 2020 Gal Shashua

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
    ``` 
