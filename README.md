# Apps Repo

This is a repository of my apps 

https://ikas-mc.github.io/fdroid-repo

## Add Repo To Fdroid(not all apps)

* Copy Link , Open F-Droid , Settings >Repositories > + 

https://ikas-mc.github.io/fdroid-repo/fdroid/repo?fingerprint=A4F1C60EB4D3A8FDE4644DBAC9F9834E3C06B69E4EACF8A7FF5423339523071B


* Open This Page In Mobile Web Browser

https://ikas-mc.github.io/fdroid-repo

* Scan  QR

![qr](https://ikas-mc.github.io/fdroid-repo/repo-qr.svg)


## For dev
Setup an F-Droid App Repo

https://f-droid.org/zh_Hans/docs/Setup_an_F-Droid_App_Repo/

```
fdroid init

keytool -genkey -keystore ikas -alias your -keyalg RSA -keysize  4096 -sigalg SHA256 withRSA -validity  10000  -storetype pkcs12   -dname "CN=your" -J-Duser.language=en

vim config.yml 

fdroid update  -c --pretty  --rename-apks
```