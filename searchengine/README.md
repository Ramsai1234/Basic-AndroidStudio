# Ex.No:6 Build a program to create a first display screen of any search engine using Auto Complete Text View.

## AIM:

To develop a program to create a first display screen of any search engine using AutoComplete TextView in Android Studio.

## EQUIPMENTS REQUIRED:

Android Studio(Min.required Artic Fox)

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as searchengine and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout using AutoComplete TextView in activity_main.xml.

Step 6: Display screen of search engine in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
Program to print the text “display screen of any search engine”.
Developed by:P.Ramsai
Registeration Number :212221240041
```
## MainActivity.java:
```
package com.example.screentext;



import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.ArrayAdapter;
import android.widget.AutoCompleteTextView;

public class MainActivity extends AppCompatActivity {
    AutoCompleteTextView autocomplete;

    String[] arr = { "Bing","youtube","Google","Yandex","Yahoo","DuckDuckGo","Swisscows","StartPage","Gibiru"};

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        autocomplete = (AutoCompleteTextView)
                findViewById(R.id.autoCompleteTextView1);

        ArrayAdapter<String> adapter = new ArrayAdapter<String>
                (this,android.R.layout.select_dialog_item, arr);

        autocomplete.setThreshold(2);
        autocomplete.setAdapter(adapter);
    }
}

```

## activity_main.xml:
```
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="@color/blue"
    android:padding="5dp"
    tools:context=".MainActivity">


    <AutoCompleteTextView
        android:id="@+id/autoCompleteTextView1"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_below="@+id/textView2"
        android:layout_centerHorizontal="true"
        android:layout_marginStart="30dp"
        android:layout_marginTop="30dp"
        android:layout_marginEnd="30dp"
        android:layout_marginBottom="30dp"
        android:ems="10"
        android:hint="Search Engine"
        android:textAlignment="center"
        tools:ignore="UnknownId" />

</RelativeLayout>

```

## OUTPUT

![Screenshot 2022-11-04 185356](https://user-images.githubusercontent.com/94269989/199984012-f38436b8-e5de-4197-94e3-930e8a996552.png)
![Screenshot 2022-11-04 185423](https://user-images.githubusercontent.com/94269989/199984044-760ee4ce-8da5-4a7e-9b13-c0111d87bd5b.png)
![Screenshot 2022-11-04 185500](https://user-images.githubusercontent.com/94269989/199984073-34c578fe-73dc-49e6-904b-c9feed1a7a48.png)



## RESULT
Thus a Simple Android Application develop a program to create a first display screen of any search engine using AutoComplete TextView in Android Studio is developed and executed successfully.
