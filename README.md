# HelloAndroid

The first project in Udacity’s Google Developer Challenge Scholarship: Android Basics – a simple Udacity card.

It’s scrollable – mostly to show everything in the landscape mode. In the portrait mode – it depends on a phone. At opening on my phone I cannot see the last sentence, when scrolling the card it’s a kind of surprise to see some additional information.

Here is the screenshot (more in a adequate directory):
https://github.com/eovka/HelloAndroid/blob/master/HelloAndroid-screenshots/HelloAndroid-Screenshot_20180128-211013.png

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
        android:layout_height="wrap_content"
        android:orientation="vertical">

        <ImageView
            android:layout_width="match_parent"
            android:layout_height="@dimen/image_size"
            android:layout_weight="1"
            android:contentDescription="@string/image_description"
            android:scaleType="centerCrop"
            android:src="@drawable/programming" />

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="@color/colorPrimaryText"
            android:orientation="horizontal">

            <TextView
                android:id="@+id/learn_text"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_gravity="start"
                android:layout_marginTop="@dimen/space12dp"
                android:fontFamily="serif"
                android:paddingLeft="@dimen/space16dp"
                android:paddingTop="@dimen/space28dp"
                android:text="@string/learn_online"
                android:textAlignment="textStart"
                android:textColor="@color/colorSecondaryText"
                android:textSize="@dimen/text_normal" />

            <ImageView
                android:layout_width="wrap_content"
                android:layout_height="@dimen/logo_size"
                android:layout_marginBottom="@dimen/space12dp"
                android:layout_marginLeft="@dimen/space8dp"
                android:layout_marginRight="@dimen/space16dp"
                android:layout_marginTop="@dimen/space12dp"
                android:contentDescription="@string/udacity_logo"
                android:src="@drawable/udacity" />
        </LinearLayout>

        <TextView
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:fontFamily="serif"
            android:gravity="center"
            android:paddingBottom="@dimen/space16dp"
            android:paddingTop="@dimen/space16dp"
            android:text="@string/udacity"
            android:textColor="@color/colorPrimaryText"
            android:textSize="@dimen/text_name"
            android:textStyle="bold" />

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="center"
            android:autoLink="map"
            android:fontFamily="serif"
            android:text="@string/udacity_address"
            android:textAlignment="center"
            android:textColor="@color/colorPrimaryText"
            android:textSize="@dimen/text_normal" />

        <TextView
            android:id="@+id/phone_number_textview"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="center"
            android:autoLink="phone"
            android:fontFamily="serif"
            android:paddingBottom="@dimen/space16dp"
            android:text="@string/udacity_phone"
            android:textColor="@color/colorPrimaryText"
            android:textSize="@dimen/text_normal" />

        <TextView
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:autoLink="web"
            android:fontFamily="serif"
            android:gravity="center"
            android:linksClickable="true"
            android:paddingBottom="@dimen/space16dp"
            android:paddingLeft="@dimen/space16dp"
            android:text="@string/learn_more"
            android:textColor="@color/colorPrimaryText"
            android:textSize="@dimen/text_www" />

    </LinearLayout>
</ScrollView>
