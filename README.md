# Kotlin-Extract

 [![](https://jitpack.io/v/jiang111/Kotlin-Extract.svg)](https://jitpack.io/#jiang111/Kotlin-Extract)

Kotlin-Extract is a "toolbox" for Kotlin Android developer.  like [anko](https://github.com/Kotlin/anko) , The library contains a lot of helpers for Android SDK, including, but not limited to:

### depend

Step 1. Add the JitPack repository to your build file
Add it in your root build.gradle at the end of repositories:
```
	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
```
Step 2. Add the dependency [![](https://jitpack.io/v/jiang111/Kotlin-Extract.svg)](https://jitpack.io/#jiang111/Kotlin-Extract)

```
	dependencies {
	        compile 'com.github.jiang111:Kotlin-Extract:lasted_version'
	}
```

### Feature

>* toast
```java

_toast("hello")
_long_toast("hello")

```
>* dp,sp,px
```java

_dip2px(20)
_sp2px(20)
...

```
>* sp_*
```java

sp_saveString("key","value")
sp_getString("key")
...

```
>* async
```java

val t = _async {
    Thread.sleep(3000)
    _runUI {
      hello.text = "hello"
    }
}
t.cancel()

```

>* startActivity
```java

_startActivity<Main2Activity>("id" to 5, "name" to "hello", "age" to 12, "male" to true)
...

```
>* loadColor/Drawable
```java

_loadColor(R.color.f)
_loadDrawable(R.drawable.f)
...

```

