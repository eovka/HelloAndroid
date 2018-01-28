# HelloAndroid

The first project in Udacity’s Google Developer Challenge Scholarship: Android Basics – a simple Udacity card.

It’s scrollable – mostly to show everything in the landscape mode. In the portrait mode – it depends on a phone. At opening on my phone I cannot see the last sentence, when scrolling the card it’s a kind of surprise to see some additional information.

And the xml code for a quick look:

<?xml version="1.0" encoding="utf-8"?>
<ScrollView xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="@color/colorPrimary"
    android:orientation="vertical"
    tools:context=".MainActivity">

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:orientation="vertical">

        <ImageView
            android:layout_width="match_parent"
            android:layout_height="250dp"
            android:layout_weight="1"
            android:scaleType="centerCrop"
            android:src="@drawable/programming" />

        <RelativeLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#ffffff"
            android:orientation="horizontal">

            <TextView
                android:id="@+id/learn_text"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_gravity="start"
                android:layout_marginTop="12dp"
                android:fontFamily="serif"
                android:padding="16dp"
                android:text="Learn online with"
                android:textAlignment="textStart"
                android:textColor="#101010"
                android:textSize="14sp" />

            <ImageView
                android:layout_width="wrap_content"
                android:layout_height="48dp"
                android:layout_marginBottom="12dp"
                android:layout_marginLeft="8dp"
                android:layout_marginRight="16dp"
                android:layout_marginTop="12dp"
                android:layout_toRightOf="@id/learn_text"
                android:src="@drawable/udacity" />
        </RelativeLayout>

        <TextView
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:fontFamily="serif"
            android:gravity="center"
            android:paddingBottom="16dp"
            android:paddingTop="16dp"
            android:text="Udacity"
            android:textColor="#ffffff"
            android:textSize="24sp" />

        <TextView
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:fontFamily="serif"
            android:gravity="center"
            android:paddingBottom="16dp"
            android:text="2465 Latham St \nMountain View, CA 94043 \n650-555-5555"
            android:textColor="#ffffff"
            android:textSize="14sp" />

        <TextView
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:autoLink="web"
            android:fontFamily="serif"
            android:gravity="center"
            android:linksClickable="true"
            android:paddingBottom="16dp"
            android:paddingLeft="16dp"
            android:text="Learn more at www.udacity.com."
            android:textColor="#ffffff"
            android:textSize="16sp" />

    </LinearLayout>
</ScrollView>
