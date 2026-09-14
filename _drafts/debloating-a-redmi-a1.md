---
layout: post
---
Basically the list of apps I debloated from my phone (Xiaomi Redmi A1)

- PAI - android.autoinstalls.config.Xiaomi.model (Play Auto Install, first boot)
- Camera - com.android.camera (Xiamoi Camera)
- com.android.camera.overlay (apparently unused)
- com.android.cameraextensions (extension for other apps to call)
- Chrome - com.android.chrome
- Clock - com.android.deskclock.go (Xiaomi Clock)
- Android S Easter Egg - com.android.egg (not genuinely useful to remove)
- com.android.overlay.gmssettingprovider (replaced with MicroG)
- com.android.overlay.gmstelecomm (replaced with MicroG)
- com.android.overlay.gmstelephony (replaced with MicroG)
- com.android.proviceds.partnerbookmarks (Google Chrome removed)
- SIM toolkit - com.android.stk (has no effect for me, has proven to be vulnerable)
- Google Play Store - com.android.vending (replaced with Aurora Store)
- DebugLoggerUI - com.debug.loggerui (may run sometimes in background)
- Meta App Manager - com.facebook.appmanager
- Meta Services - com.facebook.services
- Meta App Installer - com.facebook.system
- Sensor Test Tool - com.fingerprints.sensortesttool (not genuinely usefol to remove)
- Browser - com.go.browser (Mi Browser)
- GFManager - com.goodix.fingerprint (phone doesn’t even have a fingerprint sensor)
- Fingerprint test - com.goodix.gftest (same as above)
- Google Assistant Go - com.google.android.apps.assistant
- Google Maps - com.google.android.apps.maps
- Google Messages - com.google.android.apps.messaging (according to andorid debloat list, may require factory reset to re-acquire)
- Google Gallery Go - com.google.android.apps.photosgo
- Data Restore Tool - com.google.android.apps.restore (runs on boot)
- Google Go - com.google.android.apps.searchlite
- Search Engine Selector - com.google.android.apps.setupwizard.searchselector (runs on boot)
- Google One - com.google.android.apps.subscriptions.red
- Digital Wellbeing - com.google.android.apps.wellbeing
- Google Calendar - com.google.android.calendar 
- Google Contacts - com.google.android.contacts
- Google Dialer - com.google.android.dialer 
- Market Feedback Agent - com.google.android.feedback (doesn’t run in background)
- Gmail - com.google.android.gm
- Google Location History - com.google.android.gms.location.history (actually an empty app)
- com.google.android.gms.policy_sidecar_aps (doesn’t run on its own)
- Google Services Framework - com.google.android.gsf (replaced with MicroG)
- Gboard - com.google.android.inputmethod.latin
- Google One Time Init - com.google.android.onetimeinitializer
- com.google.android.overlay.gmsconfig.common (breaks google account login on google apps)
- com.android.overlay.gmsconfig.comms (did not break PackageInstaller)
- com.google.android.overlay.gmsconfig.gallerygo (i have no idea what it is but i debloated it and my phone works)
- com.google.android.overlay.gmsconfig.gotz (geolocation timezone detection, no effect of removal)
- com.android.overlay.gmsconfig.go (i have on idea what it is)
- com.google.overlay.gmsconfig.searchgo (i have no idea what it is)
- Google Partner Setup - com.google.android.partnersetup (no bad effect)
- Google Voice Services - com.google.android.tts
- Android System Webview - com.google.android.webview (did not work upon flashing Magisk, replaced with Bromite System WebView)
- YouTube - com.google.android.youtube
- Mi Feedback - com.miui.bugreport
- Mi Cleaner - com.miui.cleaner.go 
- Package Installer - com.miui.global.packageinstaller (did not cause bootloop, despite being on an european ROM. removes "virus check")
- Mi Music - com.miui.player
- Mi Video - com.miui.videoplayer
- com.miui.videoplayer.overlay (removed Mi Video)
- silead manager - com.silead.fingerprint (for fingerprint stuff, phone does not even have a sensor)




REMOVE CAREFULLY
- GoLauncher - com.gogo.launcher (Xiaomi launcher, handles recent apps list)
- Google Play Services - com.google.android.gms (replaced with MicroG services, need "find my device" to be removed from device admin)
- Carrier Services - com.google.android.ims (i have it installed with stock version but disabled in daily use, fully debloating removes VoLTE and VoWiFi)
- System App Updater - com.xiaomi.discover (not traditionally debloated but disabled instead, i don’t remember why but I needed it once)
