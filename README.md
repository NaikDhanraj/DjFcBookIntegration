# DjFcBookIntegration

Step 1: Creating an android project.


Step 2: Adding Dependency to your project

       --> compile 'com.facebook.android:facebook-android-sdk:4.7.0' .
       
       
Step 3: Registering our app with the facebook .com

           -->Go to developers.facebook.com/apps
           
           
Step 4 : Getting the  Hash Key

          -->   cd Program Files\Java\jre1.8.0_65\bin
          
          -->keytool -exportcert -alias androiddebugkey -keystore "C:\Users\dhanrajnaik522\.android\debug.keystore" | openssl                  sha1 -binary | openssl base64
         
          -->Add the internet permission
         
          -->Add a meta-data element to the application element
         
          -->Copy your app id and create a string resource with the name
          

 Step 5: To use Facebook Login or Share, also add the FacebookActivity  to the manifest
 
       -->        <activity android:name="com.facebook.FacebookActivity"
                  android:configChanges="keyboard|keyboardHidden|screenLayout|screenSize|orientation"
                  android:theme="@android:style/Theme.Translucent.NoTitleBar"
                  android:label="@string/app_name" />
                  
        --><application android:name=".Application"
             <meta-data android:name="com.facebook.sdk.ApplicationId"
                        android:value="@string/facebook_app_id"/>

           </application>
           
