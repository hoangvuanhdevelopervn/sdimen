# Sdimen - A scalable size unit  


  [![](https://jitpack.io/v/hoangvuanhdevelopervn/sdimen.svg)](https://jitpack.io/#hoangvuanhdevelopervn/sdimen)

- An android SDK that provides a new size unit - sdp (scalable dp). This size unit scales with the screen size. It can help Android developers with supporting multiple screens.  

- Use it carefully! for example, in most cases you still need to design a different layout for tablets.



![dp example](https://firebasestorage.googleapis.com/v0/b/contact-15400.appspot.com/o/Images%2FScreenshots%2FScreenshot_2020-08-11-20-30-32-787_com.hvasoftware.hdimensions.jpg?alt=media&token=4a480acf-e702-495d-abad-d58d094bc116)



![GitHub Logo](https://firebasestorage.googleapis.com/v0/b/contact-15400.appspot.com/o/Images%2FScreenshots%2FScreenshot_2020-08-11-20-30-38-199_com.hvasoftware.hdimensions.jpg?alt=media&token=018a2c7e-ed0e-4fc7-86fc-48cf13b79d87)


You can see that sdp scales with the screen size and the dp stays with the same size on all screen sizes.


# Gradle Dependency

### Repository

The Gradle dependency is available via [scalable dimens](https://jitpack.io/#hoangvuanhdevelopervn/sdime).

To use JitPack repository you need to add to your root build.gradle line that it at the end of repositories:

```gradle
allprojects {
    repositories {
	... 
        maven { url 'https://jitpack.io' }
    }
}
```

And as next step add dependency to project:

```gradle
dependencies  {
    implementation 'com.github.hoangvuanhdevelopervn:sdimen:1.0'
}
```


  
  # Usage


Creating simple view and use this library

```xml
<TextView  
  android:id="@+id/textview_first"  
  android:layout_width="wrap_content"  
  android:layout_height="wrap_content"  
  android:layout_marginTop="@dimen/_16sdp"  
  android:text="@string/hello_first_fragment"  
  android:textSize="@dimen/_16ssp"  
  android:textColor="#F44336"  
  />
```


---
That's it.
  
  
# Note  
The sdp size unit calculation includes some approximation due to some performance and usability constraints.
