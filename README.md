# first-android-app
![TheMaster](https://github.com/Albert-Osei/first-android-app/blob/main/appdemo.png)

It uses a BitmapShader and *does not*:
* create a copy of the original bitmap
* use a clipPath (which is neither hardware accelerated nor anti-aliased)
* use setXfermode to clip the bitmap (which means drawing twice to the canvas)

Gradle
------

dependencies {
    ...
    implementation 'androidx.core:core-ktx:1.3.0'
    implementation 'androidx.appcompat:appcompat:1.1.0'
    implementation 'androidx.constraintlayout:constraintlayout:1.1.3'
    implementation 'com.google.android.material:material:1.4.0'
}


 Usage
-----
xml
 <ImageView
        android:id="@+id/imageView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_centerInParent="true"
        android:contentDescription="@string/image_description"
        app:srcCompat="@drawable/happynewyear" />
		


License
-------

    Copyright 2022 - 2023 Albert
