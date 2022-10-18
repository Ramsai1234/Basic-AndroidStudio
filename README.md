# Basic-AndroidStudio
## Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.
## AIM:
To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:
Android Studio(Min.required Artic Fox)

## ALGORITHM:
 Step 1: Open Android Stdio and then click on File -> New -> New project.

 Step 2: Then type the Application name as HelloWorld and click Next.

 Step 3: Then select the Minimum SDK as shown below and click Next.

 Step 4: Then select the Empty Activity and click Next. Finally click Finish.

 Step 5: Design layout in activity_main.xml.

 Step 6: Display message give in MainActivity file.

 Step 7: Save and run the application.
## Program:
```
Developed by : P.Ramsai
Reg no : 212221240041
```

## MainActivity.java:
```
package com.example.helloworld;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "OnCreate Executed", Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStart(){
        super.onStart();
        Toast toast=Toast.makeText(getApplicationContext(),"OnStart Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onResume(){
        super.onResume();
        Toast toast=Toast.makeText(getApplicationContext(),"OnResume Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onPause(){
        super.onPause();
        Toast toast=Toast.makeText(getApplicationContext(),"OnPause Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStop(){
        super.onStop();
        Toast toast=Toast.makeText(getApplicationContext(),"OnStop Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onRestart(){
        super.onRestart();
        Toast toast=Toast.makeText(getApplicationContext(),"OnRestart Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onDestroy(){
        super.onDestroy();
        Toast toast=Toast.makeText(getApplicationContext(),"OnDestroy Executed",Toast.LENGTH_LONG);
        toast.show();
    }
}
```
## activity_main.xml:
```<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="HelloWorld!"
        android:layout_centerVertical="true"
        android:layout_centerHorizontal="true"
        android:textSize="20sp"
        android:textColor="@color/black"

        />
</RelativeLayout>
```
## Output:
![Screenshot (173)](https://user-images.githubusercontent.com/94269989/196340955-dfc74716-2dbf-4d08-be0f-010866080829.png)

![Screenshot (174)](https://user-images.githubusercontent.com/94269989/196341070-832e0fa8-bb55-47ec-b464-e7c6fa1aa1ca.png)
![Screenshot (175)](https://user-images.githubusercontent.com/94269989/196341163-72c1f63e-e8c7-4998-b76f-c89027056d98.png)
![Screenshot (176)](https://user-images.githubusercontent.com/94269989/196341255-22326604-9828-4e31-b53c-6f31df399c70.png)
![Screenshot (177)](https://user-images.githubusercontent.com/94269989/196341411-51ab7232-fc9b-4bcc-a2b4-d27720a55cd1.png)
![Screenshot (178)](https://user-images.githubusercontent.com/94269989/196341450-d4241bbf-c47e-4ecc-9a66-b5618d924521.png)
![Screenshot (179)](https://user-images.githubusercontent.com/94269989/196341590-5e66f403-0055-4c5e-96d1-c76e173992a5.png)




## Result:
Therefore a program is return to develop a program to detect the various life cycles of an activity. The program is successfully executed.










