GradientView 🌈
=================

<img src="/preview/preview.gif" alt="sample" title="sample" width="300" height="480,62" align="right" vspace="52" />

[![Platform](https://img.shields.io/badge/platform-android-green.svg)](http://developer.android.com/index.html)
[![API](https://img.shields.io/badge/API-16%2B-brightgreen.svg?style=flat)](https://android-arsenal.com/api?level=16)
<br>
[![Twitter](https://img.shields.io/badge/Twitter-@LopezMikhael-blue.svg?style=flat)](http://twitter.com/lopezmikhael)

This is an Android project allowing to realize a gradient View in the simplest way possible. Finish the gradient shapes of all colors in your projects.

<a href="https://play.google.com/store/apps/details?id=com.mikhaellopez.lopspower">
  <img alt="Android app on Google Play" src="https://developer.android.com/images/brand/en_app_rgb_wo_45.png" />
</a>

USAGE
-----

To make a gradient View add GradientView in your layout XML and add GradientView library in your project or you can also grab it via Gradle:

:information_source: **PUBLICATION IN PROGRESS**

```groovy
implementation 'com.mikhaellopez:gradientview:1.0.0'
```

XML
-----

```xml    
<com.mikhaellopez.gradientview.GradientView
    android:id="@+id/gradientView"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    app:gv_direction="left_to_right"
    app:gv_end="#d32e2e"
    app:gv_start="#3f51b5" />
```

You must use the following properties in your XML to change your CircleView.

| Properties           | Type                                                         | Default       |
| -------------------- | ------------------------------------------------------------ | ------------- |
| `app:gv_start`       | color                                                        | WHITE         |
| `app:gv_alpha_start` | float (from 0.0 to 1.0)                                      | 1f            |
| `app:gv_end`         | color                                                        | WHITE         |
| `app:gv_alpha_end`   | float (from 0.0 to 1.0)                                      | 1f            |
| `app:gv_direction`   | left_to_right, right_to_left, top_to_bottom or bottom_to_top | left_to_right |

KOTLIN
-----

```kotlin
val gradientView = findViewById<GradientView>(R.id.gradientView)
gradientView.apply {
    // Set Color Start
    start = Color.RED
    alphaStart = 0.5f
    
    // Set Color End
    end = Color.BLUE
    alphaEnd = 0.5f
    
    // Set Gradient Direction
    direction = GradientView.GradientDirection.TOP_TO_BOTTOM
}
```

JAVA
-----

```java
GradientView gradientView = findViewById(R.id.gradientView);

// Set Color Start
gradientView.setStart(Color.RED);
gradientView.setAlphaStart(0.5f);

// Set Color End
gradientView.setEnd(Color.RED);
gradientView.setAlphaEnd(0.5f);

// Set Gradient Direction
gradientView.setDirection(GradientView.GradientDirection.TOP_TO_BOTTOM);
```

LICENCE
-----

CircleView by [Lopez Mikhael](http://mikhaellopez.com/) is licensed under a [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0).
