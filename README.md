# Project6_H_2
SlidingDrawer 사용 

손잡이를 당기면 속 서랍이 나오도록 함

![Project6_H_2](https://user-images.githubusercontent.com/37572367/88132958-d0f32380-cc1b-11ea-84a8-94484539c9c1.PNG)

<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical" >

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="여긴 서랍 밖입니다"
        android:textSize="20dp"/>

    <SlidingDrawer
        android:id="@+id/slidingdrawer"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:content="@+id/content"
        android:handle="@+id/handle"
        android:orientation="vertical" >

        <Button
            android:id="@+id/handle"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="서랍 손잡이"
            android:textSize="20dp"/>

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:id="@+id/content"
            android:background="#4CAF50"
            android:orientation="vertical" >

            <SlidingDrawer
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:content="@+id/content2"
                android:handle="@+id/handle2"
                android:orientation="vertical"
                android:topOffset= "200dp" >

                <Button
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:id="@+id/handle2"
                    android:background="#079F0D"
                    android:text="안 서랍 손잡이"
                    android:textSize="20dp"/>

                <LinearLayout
                    android:id="@+id/content2"
                    android:layout_width="match_parent"
                    android:layout_height="match_parent"
                    android:orientation="vertical"
                    android:background="#D10AF3"
                    android:gravity="center|bottom" >

                    <TextView
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:text="여긴 두번쨰 서랍 안 입니다"
                        android:textSize="20dp" />

                </LinearLayout>

            </SlidingDrawer>
        </LinearLayout>
    </SlidingDrawer>


</LinearLayout>
