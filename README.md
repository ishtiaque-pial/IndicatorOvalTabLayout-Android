Setup
----------------

First, add jitpack in your build.gradle at the end of repositories:
 ```gradle
repositories {
    // ...       
    maven { url "https://jitpack.io" }
}
```

Then, add the library dependency:
```gradle
compile 'com.github.ishtiaque-pial:IndicatorOvalTabLayout-Android:v1.3'
```

Now go do some awesome stuff!

Usage
----------------

```xml
 <com.pial.indicatorovaltablayout.TabLayoutWithOval
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        ></com.pial.indicatorovaltablayout.TabLayoutWithOval>
```

```java
TabLayoutWithOval tabLayout = (TabLayoutWithOval)findViewById(R.id.tabLayout);
        ViewPager viewPager = (ViewPager)findViewById(R.id.viewPager);
        viewPager.setAdapter(new PagerAdapter(getSupportFragmentManager(), fragments));
        tabLayout.setupWithViewPager(viewPager);
```
Licence
----------------
The MIT License (MIT)

Copyright (c) 2017 Ishtiaque Morshed
