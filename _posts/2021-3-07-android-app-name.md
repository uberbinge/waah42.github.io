---
layout: post
title: Android app name not showing up
permalink: android-app-name-not-showing-up
---

Recently I learned that if you specify a title for your "Main" `activity`, the app drawer shows that title under App-icon instead of the "app_name" provided in `application`tag. Which may not be the desired/expected behavior for some.

## Before
With following code the app drawer shows `activity` label in app drawer and application label in App's info page.

```xml
   <application
        android:name=".WhereIsMyMoneyApp"
        android:allowBackup="true"
        android:icon="@mipmap/ic_launcher"
        android:label="Where is my money" 
        android:supportsRtl="true"
        android:theme="@style/AppTheme">
        <activity
            android:name=".MainActivity"
            android:label="Transactions"
            android:screenOrientation="portrait">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />
                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
```
<a href="/images/with-activity-label.png"><img src="../assets/img/with-activity-label.png" alt="The view of app drawer when acitivity label is provided"></a>

## After
After removing `activity's` `android:label` now both app drawer and App's info page show same name.

```xml
        <activity
            android:name=".MainActivity"
            android:screenOrientation="portrait">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />
                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
```
<a href="/images/without-activity-label.png"><img src="../assets/img/without-activity-label.png" alt="The view of app drawer when acitivity label is provided"></a>

### Tip
Avoid giving your “Main” `activity` `android:label="@string/any_name"` if you don’t want that name to end up in App drawer. 
