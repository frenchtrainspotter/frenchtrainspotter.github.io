---
layout: post
---
<!-- I should add more work to this paragraph, and add a part or section about 1) my de-bloater of choice and 2) the android debloat list -->
This is a list of apps I have de-bloated on my main phone, a Redmi A1 (codename ice), not to be confused with the Mi A1 (codename tissot). Please note that because this is safe on my phone doesn’t mean it will be on other Xiaomi phones.

## Why I de-bloated my phone in the first place
<!-- I should find a way to display an image on the side -->
<!-- I should also add actual text to this -->
![A Screenshot of the Xiaomi Clock app provided with Android 12 Go devices. The pop-up is in French and reads "Dans le but d’offrir des services personnalisés, Horloge doit se connecter à internet. Avant d’utiliser l’horloge, vous devez aussi lire et accepter notre Accord Utilisateur et Politique de Confidentialité. Accepter?". It has a button to not ask anymore, and buttons to refuse or accept](/assets/images/debloating-a-redmi-a1_img1.png)

## Google packages
### Apps
Google apps. Includes apps that may not have "Google" in their name.
- Chrome (com.android.chrome)
  - Browser replaced with [Fennec F-Droid](https://f-droid.org/packages/org.mozilla.fennec_fdroid/) (Firefox)
- Gboard - com.google.android.inputmethod.latin
  - Replaced with [AnySoftKeyboard](https://f-droid.org/en/packages/com.menny.android.anysoftkeyboard/)
- Gmail - com.google.android.gm
  - Replaced with [K-9 Mail](https://f-droid.org/en/packages/com.fsck.k9/)
- Google Assistant Go - com.google.android.apps.assistant
- Google Calendar - com.google.android.calendar 
  - Replaced with [Etar](https://f-droid.org/en/packages/ws.xsoh.etar/)
- Google Contacts - com.google.android.contacts
  - Replaced with [Fossify Contacts](https://f-droid.org/en/packages/org.fossify.contacts/)
- Google Gallery Go - com.google.android.apps.photosgo
  - Replaced with [Fossify Gallery](https://f-droid.org/en/packages/org.fossify.gallery/)
- Google Go - com.google.android.apps.searchlite
- Google Maps - com.google.android.apps.maps
  - Replaced with [OsmAnd~](https://f-droid.org/en/packages/net.osmand.plus/)
- Google Messages - com.google.android.apps.messaging
  - If debloated, some features may require a factory reset to re-obtain
  - Replaced with [QUIK SMS](https://f-droid.org/en/packages/dev.octoshrimpy.quik.fdroid/)
- Google One - com.google.android.apps.subscriptions.red
- Google Phone - com.google.android.dialer 
  - Replaced with [Fossify Phone](https://f-droid.org/en/packages/org.fossify.phone/)
- Google Play Store - com.android.vending
  - Main app store replaced with [F-Droid](https://f-droid.org/) ([Droid-ify](https://f-droid.org/en/packages/com.looker.droidify/) client)
  - Play Store client replaced with [Aurora Store](https://f-droid.org/en/packages/com.aurora.store/)
- YouTube - com.google.android.youtube
  - Replaced with [PipePipe](https://f-droid.org/en/packages/InfinityLoop1309.NewPipeEnhanced/)

### Google Play Services
[According to the ADL](https://adl.muntashir.dev/bloatware/com.google.android.gms.html), it is **needed** to remove Find my devices from device admin apps before removing GMS.
You can decide to use your phone either without Play Services at all, or to replace them with [MicroG](https://github.com/microg/GmsCore/wiki/Downloads) (which is the option I went with).  
Having no Play Services at all seemed to have a notable positive impact on battery life but broke some apps.
Meanwhile, using MicroG (at least the way I set it up) removed basically all battery life gains, however you still have control over which permissions you grant, unlike stock Play Services.
- Google Play Services - com.google.android.gms
- Google Location History - com.google.android.gms.location.history
- Google Services Framework - com.google.android.gsf
- com.android.overlay.gmsconfig.comms
- com.android.overlay.gmsconfig.go
- com.android.overlay.gmssettingprovider
- com.android.overlay.gmstelecomm
- com.android.overlay.gmstelephony
- com.google.android.gms.policy_sidecar_aps
- com.google.android.overlay.gmsconfig.common
- com.google.android.overlay.gmsconfig.gallerygo
- com.google.android.overlay.gmsconfig.gotz
- com.google.overlay.gmsconfig.searchgo

### Misc packages/services
- Android System Webview - com.google.android.webview
  - Webview replaced with Bromite System WebView (using AnyWebView to set it as default)
- Carrier Services - com.google.android.ims
  - Safe to remove if you do not use VoLTE/VoWiFi, else you should only disable it
- com.android.providers.partnerbookmarks
- Data Restore Tool - com.google.android.apps.restore
- Digital Wellbeing - com.google.android.apps.wellbeing
- Google One Time Init - com.google.android.onetimeinitializer
- Google Partner Setup - com.google.android.partnersetup
- Google Voice Services - com.google.android.tts
- Market Feedback Agent - com.google.android.feedback
- Search Engine Selector - com.google.android.apps.setupwizard.searchselector

## Xiaomi apps
- Camera - com.android.camera
  - Replaced with [Open Camera](https://f-droid.org/en/packages/net.sourceforge.opencamera/)
- com.android.camera.overlay
- com.android.cameraextensions
- Clock - com.android.deskclock.go
- Mi Browser - com.go.browser
- Mi Cleaner - com.miui.cleaner.go 
- Mi Feedback - com.miui.bugreport
- Mi Music - com.miui.player
  - Replaced with [Auxio](https://f-droid.org/en/packages/org.oxycblt.auxio/)
- Mi Video - com.miui.videoplayer
  - Replaced with [VLC](https://f-droid.org/en/packages/org.videolan.vlc/)
- com.miui.videoplayer.overlay
- Package Installer - com.miui.global.packageinstaller
  - ADL warns about bootloop after removal on Xiaomi EU ROMs. My phone does, in fact, not bootlop. Maybe it only applies to MIUI?
- Play Auto Installs - android.autoinstalls.config.Xiaomi.model

## Other apps
- Android S Easter Egg - com.android.egg (not genuinely useful to remove)
- DebugLoggerUI - com.debug.loggerui (may run sometimes in background)
- SIM toolkit - com.android.stk (has no effect for me, has proven to be vulnerable)

### Fingerprint stuff
Self-explanatory, the phone doesn’t even have a fingerprint sensor.
- Fingerprint test - com.goodix.gftest (same as above)
- GFManager - com.goodix.fingerprint
- Sensor Test Tool - com.fingerprints.sensortesttool
- silead manager - com.silead.fingerprint (for fingerprint stuff, phone does not even have a sensor)

### Exec at boot
Apps that *should* only execute on boot (includes first boot apps).

### Meta/Facebook stuff
- Meta App Installer - com.facebook.system
- Meta App Manager - com.facebook.appmanager
- Meta Services - com.facebook.services

## Honourable mentions

REMOVE CAREFULLY
- GoLauncher - com.gogo.launcher (Xiaomi launcher, handles recent apps list)
- System App Updater - com.xiaomi.discover (not traditionally debloated but disabled instead, i don’t remember why but I needed it once)
