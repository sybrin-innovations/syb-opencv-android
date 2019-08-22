# opencv for android

dependencies {

  // opencv 3.4.1
  opencv:3.4.1'
  
  // opencv 3.4.4 with contribution packages
  opencv:3.4.4-contrib'
  
  // opencv 3.4.5
  opencv:3.4.5'
 
  // opencv 4.0.1
  opencv:4.0.1'
  
  // opencv 4.1.0
  opencv:4.1.0'
  
  // opencv 4.1.0 with contribution packages
   opencv:4.1.0-contrib'
}
```

and this in your project's build.gradle **repositories** section
```groovy
repositories {
  jcenter()
}
```

Don't forget to also initialize OpenCV with a statement like this e.g. in your Application class:
```kotlin
if (!OpenCVLoader.initDebug())
   Log.e("OpenCv", "Unable to load OpenCV");
else
   Log.d("OpenCv", "OpenCV loaded");
```

