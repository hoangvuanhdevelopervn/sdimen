# Scalable Dimens - A scalable size unit  
- An android SDK that provides a new size unit - sdp (scalable dp). This size unit scales with the screen size. It can help Android developers with supporting multiple screens.  


# Gradle Dependency

### Repository

The Gradle dependency is available via [Scalable-Dimensions](https://jitpack.io/#hoangvuanhdevelopervn/Scalable-Dimensions).

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
    implementation 'com.github.hoangvuanhdevelopervn:Scalable-Dimensions:-SNAPSHOT'
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