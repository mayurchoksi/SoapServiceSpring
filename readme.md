Create a keystore

cd /tmp
keytool -genkey -alias tomcat -storetype PKCS12 -keyalg RSA -keysize 2048 -keystore keystore.p12 -validity 3650

Add the keystore details into the application properties (application.yml)
update src/main/java/application.yml with the the keystore location and password