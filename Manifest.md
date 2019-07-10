##

1. Activity
  <application ... >
    <activity android:name="com.jessicathornsby.myapplications.ShareActivity">
  </application ... >

2 .Services

       </activity>
     <service
   android:description="@string/servicedesc"
   android:name=".MyService">
</service>
   </application>

</manifest>

3. Broadcast Receiver

<receiver android:name=".MyBroadcastReceiver”">
  <intent-filter>
    <action android:name="android.intent.action.ACTION_POWER_CONNECTED"/>
  </intent-filter>
</receiver>

4. Implicit intents

//This Activity is the main entry point into your app//

<activity android:name="MainActivity">
    <intent-filter>
        <action android:name="android.intent.action.MAIN" />
        <category android:name="android.intent.category.LAUNCHER" />
    </intent-filter>
</activity>

<activity android:name="CallActivity">
    <intent-filter>

//The action that this component will accept//

    <action android:name="android.intent.action.CALL"/>

//The intent category that this component will accept//

    <category android:name="android.intent.category.DEFAULT"/>

//The type of data this component will accept, such as scheme, host, port, or path//

        <data android:mimeType="text/plain"/>
    </intent-filter>
</activity>
