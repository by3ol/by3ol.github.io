---

title:  "The Complete Android Java Developer Course:2023"
author: by3ol
date: 2023-09-25 11:33:00 +0800
categories: [Lecture]
tags: [udemy]
pin: true
math: true
mermaid: true
---



## Section 27: Dagger2

* ####  One class is dependent on the other classes , One class can’t exist without other classes : hard dependency
* ####  We can eliminate hard dependency using manual Dependency Injection and Dagger2.


## Section 28 : Android Content Provider

* ####  Check permission and request permission
```java
if(ContextCompat.checkSelfPermission(this, Manifest.permission.READ_CONTACTS) != PackageManager.PERMISSION_GRANTED){ 
    ActivityCompat.requestPermissions(this,new String[]{Manifest.permission.READ_CONTACTS},RCREQUESTCODE);
}
```
* ####  OnRequestPermissionResult will be executed when the user respond to the dialog of the permission
* ####  How to adjust image to center of imagebutton
```xml
android:adjustViewBounds="true"
android:scaleType="fitCenter"
```
* ####  How to get contact
```java
 Uri uri = ContactsContract.CommonDataKinds.Phone.CONTENT_URI;
 Cursor cursor = contentResolver.query(uri,null,null,null,null);
```
* #### Four main Android app components 
→ activities, services, content providers, and broadcast receivers.


## Section 30 : Calculator Apps


* #### What I learned in this course 

    * How to use addTextChangeListener on TextEditor
    * How to use setOnSeekBarListener on SeekBar

* #### How to change button color
```
app:backgroundTint="@null"
```
* #### Parent component's gravity attribute affects child's location 


## Section 31 :  Master Location Services In Android

* ####  How to use Google Map in Android 
Get API key and use Google Maps Views Activity

* ####  How to get fine location permission
```java
 ActivityCompat.requestPermissions(this,new String[]{Manifest.permission.ACCESS_FINE_LOCATION},FINE_LOCATION_REQUEST_CODE);
```
* ####  FusedLocationProviderClient : getLastLocation 
→ Returns most recent location

* #### GoogleMap : setMyLocationEnable 
→ Continuously draws an indication of a user’s current location

## Section 33 :  Exoplayer Media Application Development

* ####  What I learned in this course 

    * How to play music with exoplayer
    * How to customize user interface of exoplayer
    * How to get permission with Dexter library
    * How to download music with uri 

* #### How to download music 
→ Use DownloadManager

## Section 34 :  Android Media App Development 

* #### What I learned in this course

    * How to use animation in Android
    * How to play music and video in Android
    * How to change volume in Android
    * How to move back and forth while playing music
    * How to use Timer

* #### How to set view component’s location 
 → Use setX(), setY()

* #### How to get child component’s number and child components
→ getChildCount(), getChildAt()

* #### How to play music in Android
→ Use MediaPlayer

* #### How to play video in Android
→ Connect uri to videoview

* #### Timer
→ Using a timer, we can execute some work repeatedly in the background.

* #### MediaPlayer

    * start() : play music
    * pause() : stop music
    * getCurrentPosition() : return current position
    * seekTo() : move to certain position 
    * setOnCompletionListener() : set onCompletionListener  


