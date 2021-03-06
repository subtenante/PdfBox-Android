PdfBox-Android
==============
[ ![Download](https://api.bintray.com/packages/birdbrain2/PdfBox-Android/PdfBox-Android/images/download.svg) ](https://bintray.com/birdbrain2/PdfBox-Android/PdfBox-Android/_latestVersion)

A port of Apache's PdfBox library to be usable on Android. Most features should be implemented by now. Feature requests can be added to the issue tracker. Stable releases can be added as a Gradle dependency from jcenter.

The main code of this project is licensed under the Apache 2.0 License, found at http://www.apache.org/licenses/LICENSE-2.0.html Any code released under a different licenses will be stated in the header.

Usage
==============

Add the following to dependency to `build.gradle`:

```gradle
dependencies {
    compile 'com.tom_roush.pdfbox-android:1.8.9.1'
}
```

Before calls to PDFBox are made it is **highly** recommended to initialize the library's resource loader. Add the following line before calling PDFBox methods:

```java
PDFBoxResourceLoader.init(getApplicationContext());
```

An example app is located in the `sample` directory and includes examples of common tasks.

Important notes
==============

-Currently based on PdfBox v1.8.9

-This is still a work in progress

Libraries
==============
PDFBox-Android depends on the following libraries: SpongyCastle core, prov, and pkiv: https://github.com/rtyley/spongycastle/
