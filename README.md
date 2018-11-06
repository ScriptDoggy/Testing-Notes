## Android - Sign Unsigned APKs (Self-signed)
Step 1: set path C:\Program Files (x86)\Java\jdk1.8.0_20\bin in command line

Step 2: jarsigner -verbose -keystore /path_to_keystore/keystoreFileName  /path_to_apk_file/application_name.apk keystoreFileName_alias

-keystoreFileName_alias. You have to provide your alias name of your keystore file name.

Step 3: Enter password of your keystore file

Step 4: Completed. It will displays warning messages like certifaction validity etc..

Step 5: Verify your apk file jarsigner -verify /path_to_apk_file/application_name.apk

Zip align:

Step 6: set path C:\Program Files (x86)\Android\sdk\build-tools\android-4.4W in command line

Step 7: zipalign -v 4 /path_to_apk_file/application_name.apk /path_to_destination_apk_locaion/zipped_application_name.apk
