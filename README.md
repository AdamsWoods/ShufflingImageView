# ShufflingImageView

---------------------

<img src="https://i.loli.net/2020/08/08/irMQuBN53ZtLAIb.png" alt="shuffling_1.png" style="zoom:25%;" /> 

[![](https://jitpack.io/v/Edward7Zhang/ShufflingImageView.svg)](https://jitpack.io/#Edward7Zhang/ShufflingImageView)

## What's this

This widget can move your picture like a *Shuffling flow poster* 

### Feature:

* Easy used
* Very smooth
* Custom picture number
* Custom moving speed
* Custom color split line
* Custom placeholder

### Later feature:

* Custom moving direction
* Custom ...

## How 2 use

### Add dependency

Add it in your root build.gradle at the end of repositories:

**Step 1.** Add the JitPack repository to your build file

```groovy
	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
```

**Step 2.** Add the dependency

```groovy
	dependencies {
	        implementation 'com.github.Edward7Zhang:ShufflingImageView:v1.0.0'
	}
```

### Use it

**In xml Layout**

```xml
<com.majortom.library.ShufflingImageView
            android:id="@+id/shuffling_image_view"
            android:layout_width="match_parent"
            android:layout_height="match_parent" />
```

```java
mShuffingImageView = findViewById(R.id.shuffling_image_view);
mShuffingImageView.setSpeed(1);
mShuffingImageView.setImagePlaceholder(R.drawable.placeholder1, 6);
mShuffingImageView.setImagePathList(thumbList);
```

**Or new it**

```
mShuffingImageView = new ShufflingImageView(this);
mShuffingImageView.setSpeed(1);
mShuffingImageView.setImagePlaceholder(R.drawable.placeholder1, 6);
mShuffingImageView.setImagePathList(thumbList);
```

... then add it in your layout

<img src="https://i.loli.net/2020/08/08/86WxVuSyd9ja3XL.png" alt="shuffling_2.png" style="zoom:70%;" />

**More information see Demo please😉**