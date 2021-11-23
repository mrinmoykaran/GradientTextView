<h1 align="center">GradientTextView</h1></br>
<p align="center">
<img src="https://github.com/mrinmoykaran/GradientTextView/blob/master/GradientTextView1.jpg" width="450" />
<br>
  A easy to use android library to apply gradient effect on plain TextView.
</p>
<h6 align="center">
 <img src="https://img.shields.io/badge/Android-GradientTextView-blue.svg" height="22" valign="middle">&nbsp;&nbsp;
 <img src="https://img.shields.io/github/forks/mrinmoykaran/gradienttextview?style=social" height="22" valign="middle">&nbsp;&nbsp;
 <img src="https://img.shields.io/badge/API-21%2B-brightgreen.svg?style=flat" height="22" valign="middle">&nbsp;&nbsp;
 <img src="https://jitpack.io/v/mrinmoykaran/GradientTextView.svg" height="22" valign="middle">&nbsp;&nbsp;
 <img src="https://img.shields.io/badge/Platform-Android-brightgreen.svg" height="22" valign="middle">&nbsp;&nbsp;
 <img src= "https://avatars.githubusercontent.com/u/25265062?s=64&v=4" height="22" valign="middle">&nbsp;&nbsp;By <a href="linkedin.com/in/mrinmoykaran/">Mrinmoy Karan</a>
</h6>

## Contents
- [Getting started](#getting-started)
- [Attribute Description](#attribute-description)
- [Usage](#usage)
- [Limitation](#Limitation)

## Getting started

### Using Gradle
---

*Versions 1.0.0 can only be used with jitpack, versions 1.1.0 and up can be used with Maven Central.*

**Step 1 :** Add it in your root `build.gradle` at the end of repositories.
```xml
   allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
```

**Step 2 :** This library is available on jitpack,maven it by adding the following dependency to your <b>build.gradle</b>:
```gradle

implementation 'com.github.mrinmoykaran:GradientTextView:1.0.0'

```

**Step 3 :** Define `GradientTextView` in your XML layout with custom attributes.
```xml
    <com.mrinmoy.karan.GradientTextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="HELLOW WORLD!"
        android:textSize="50sp"
        android:textStyle="bold"
        android:id="@+id/gradienttextview1"
        app:startColor="#FFEB3B"
        app:centerColor="#FF9800"
        app:endColor="#FF5722"
        app:angle="45"/>
```
### Using Maven
---
**Step 1 :** Add the JitPack repository to your build file.
```
   <repositories>
	<repository>
           <id>jitpack.io</id>
	   <url>https://jitpack.io</url>
	</repository>
   </repositories>
```

**Step 2 :** This library is available on jitpack,maven it by adding the following dependency to your <b>build.gradle</b>:
```
    <dependency>
     <groupId>com.github.mrinmoykaran</groupId>
	<artifactId>GradientTextView</artifactId>
      <version>Tag</version>
    </dependency>

```

## Attribute Descriptions


| Attribute  | Description |
| :-- | :-- |
| startColor  | This is the starting color of the gradient. This color will start from the top of the `GradientTextView`.  |
| centerColor | This color will come in the center of the `GradientTextView`  |
| endColor    | This is the ending color of the 1GradientTextView` |
| angle       | The angle for the gradient, in degrees. 0 is left to right, 90 is bottom to top. It must be a multiple of 45. Default is 0. |

## Limitation of the Library

### Required
You need to declare all the four attributes( `startColor` , `centerColor` , `endColor` , `angle` ), without any of these attribute can crash the app.
