# Android Basics Workshop

## Java / Kotlin refresher
`
To add here
`
## Installation
`
To add here
`

## Android Manifest
```
<manifest>

   # Declaring permission
   <uses-permission android:name="...." />
   
   # Declaring activity
   <activity android:name="...."/>
   
</manifest>
```

## Activity

An activity represents a single screen with a user interface just like window or frame of Java.
```
package com.example.name;

public class MainActivity extends Activity {
   
   /** Called when the activity is first created. */
   @Override
   public void onCreate(Bundle savedInstanceState) {
      super.onCreate(savedInstanceState);
      setContentView(R.layout.activity_main);
   }

}
```

### Android Life-Cycle

#### onCreate()
You must implement this callback, which fires when the system creates your activity. Your implementation should initialize the essential components of your activity: For example, your app should create views and bind data to lists here.
When onCreate() finishes, the next callback is always onStart().

#### onStart()
As onCreate() exits, the activity enters the Started state, and the activity becomes visible to the user.

#### onResume()
The system invokes this callback just before the activity starts interacting with the user. 
The onPause() callback always follows onResume().

#### onPause()
The system calls onPause() when the activity loses focus and enters a Paused state. This state occurs when, for example, the user taps the Back or Recents button. When the system calls onPause() for your activity 
Once onPause() finishes executing, the next callback is either onStop() or onResume(), depending on what 

#### onStop()
The system calls onStop() when the activity is no longer visible to the user.
The next callback that the system calls is either onRestart(), if the activity is coming back to interact with the user, or by onDestroy() if this activity is completely terminating.

#### onRestart()
The system invokes this callback when an activity in the Stopped state is about to restart. onRestart() restores the state of the activity from the time that it was stopped.
This callback is always followed by onStart().

#### onDestroy()
The system invokes this callback before an activity is destroyed.


## Gradle
`
To add here
`

## References 
- [Official Android Developer Guide](https://developer.android.com/guide)
- [Tutorials Point Android Tutorial](https://www.tutorialspoint.com/android)
