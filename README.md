# Video Opener Library

[![](https://jitpack.io/v/GalShashua/VideoOpenerLibrary.svg)](https://jitpack.io/#GalShashua/VideoOpenerLibrary)

![screenshot0](https://user-images.githubusercontent.com/56959832/99788323-a2357d00-2b29-11eb-95f2-de9b57415958.JPG)
![screenshot2](https://user-images.githubusercontent.com/56959832/99731752-0410cb00-2ac7-11eb-8c87-dde88d4be7e2.JPG)

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

###### StepProgress Constructor:
```java

// For continual calls - 
SmartRate.Rate(MainActivity.this
        , "Rate Us"
        , "Tell others what you think about this app"
        , "Continue"
        , "Please take a moment and rate us on Google Play"
        , "click here"
        , "Ask me later"
        , "Never ask again"
        , "Cancel"
        , "Thanks for the feedback"
        , Color.parseColor("#2196F3")
        , 4
        , 48
        , 72
);

// For one time call
SmartRate.Rate(MainActivity.this
        , "Rate Us"
        , "Tell others what you think about this app"
        , "Continue"
        , "Please take a moment and rate us on Google Play"
        , "click here"
        , "Cancel"
        , "Thanks for the feedback"
        , Color.parseColor("#2196F3")
        , 4
);

// With Call Back:
SmartRate.Rate(MainActivity.this
        , "Rate Us"
        , "Tell others what you think about this app"
        , "Continue"
        , "Please take a moment and rate us on Google Play"
        , "click here"
        , "Cancel"
        , "Thanks for the feedback"
        , Color.parseColor("#2196F3")
        , 4
        , new SmartRate.CallBack_UserRating() {
            @Override
            public void userRating(int rating) {
                // Do something
                // maybe from now disable this button
            }
        }
);

// Self implement without link to google play store:
// -1 on stars
SmartRate.Rate(MainActivity.this
        , Color.parseColor("#E44643")
        , -1
        , new SmartRate.CallBack_UserRating() {
            @Override
            public void userRating(int rating) {
                Toast.makeText(MainActivity.this, "Rating: " + rating + " Stars", Toast.LENGTH_LONG).show();
                //saveUserRating(rating);
            }
        }
);

```

## License

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
    
