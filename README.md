# clear text problem with android 9 update .

**problem description :**
	

problem oucured when using android 9 .you can't use http request by default ,so you have to specify in your manifest file that you are using them by setting clear text to true .in cordova and ionic project you have to specify that one config.json

**steps for solution :**

 1. update platform android in config.json :
 

 ```
<platform name="android">
  <edit-config file="app/src/main/AndroidManifest.xml" mode="merge" target="/manifest/application">
      <application android:usesCleartextTraffic="true" />
  </edit-config>
</platform>```
```

 2. update widget in config.json
```
xmlns:android="http://schemas.android.com/apk/res/android"
```

