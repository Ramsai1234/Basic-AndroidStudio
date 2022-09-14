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
![Screenshot (100)](https://user-images.githubusercontent.com/94269989/190158931-2b915609-fe32-45f3-9706-b0ad420a24bc.png)
![Screenshot (101)](https://user-images.githubusercontent.com/94269989/190159059-f38ac9b9-05f8-4052-84c5-0255f71b8ab8.png)
![Screenshot (102)](https://user-images.githubusercontent.com/94269989/190159250-7e8a6284-9024-400c-bcca-3fc65883e2ec.png)
![Screenshot (103)](https://user-images.githubusercontent.com/94269989/190159355-62f8b44f-0ef1-4646-8617-86a7a0f44670.png)
![Screenshot (104)](https://user-images.githubusercontent.com/94269989/190159433-2302ab82-b79b-453a-b2f3-fa6b18cad2a7.png)
![Screenshot (105)](https://user-images.githubusercontent.com/94269989/190159475-db894772-1de8-4866-9dc7-18af75122c03.png)
![Screenshot (106)](https://user-images.githubusercontent.com/94269989/190159554-24f4d68e-88e7-4a34-99b3-4b2febc95bf3.png)

## Result:
Therefore a program is return to develop a program to detect the various life cycles of an activity. The program is successfully executed.










