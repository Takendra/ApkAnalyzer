# ApkAnalyzer
ApkAnalyzer picks the apk throught command line or path of the apk can be given directly to apkPath variable in MainClass.java.
the project generates the result.txt file after parsing it and if same apk is given again it finds the difference between the apks and generates the outputCompare.txt file.
the project uses mysql as database to store the apk details and make the comparision if same apk is again testd on project.
to rn the project following script for databse can be used to  creare database and required table

===========================================Database script=====================================
create database apkDb;
use apkdb;

create table apkDetails(packageName varchar(200) primary key,
apkName varchar(200),
apkSize varchar(100),
apkDexSize varchar(100),
apkResourcesSize varchar(100),
apkAssetsSize varchar(100),
apkIsDebuggable varchar(10),
apkVersionInfo varchar(2000),
apkSdkInfo varchar(2000),
apkCompiledSdkVersion varchar(100),
apkCompileSdkVersionName varchar(100),
apkSupportedScreenSize varchar(5000),
akpActivityCount varchar(100),
apkActivitiesName longtext,
apkPermissionsCount varchar(100),
apkPermissionNames longtext,
apkServiceCount varchar(100),
apkServiceNames longtext,
apkFeatureCount varchar(100),
apkFeatureNames longtext,
apkBroadCastCount varchar(100),
apkBroadCastNames longtext,
apkContentProviderCount varchar(100),
apkContentProvideNames longtext,
apkSignInfoMD5  longtext,
apkSignInfoSHA1 longtext,
apkSignInfoSHA256 longtext,
apkSignInfoFacebookHash longtext,
apkSignInfoPublicKey longtext,
apkSignInfoVersion text,
apkSignInfoSignature longtext,
apkSignInfoSignAlgName longtext,
apkSignInfoSerialNumber text,
apkSignInfoIssuerNameDn longtext,
apkSignInfoSubjectNameDn longtext,
apkSignInfoGetNotAfter text,
apkSignInfoGetNotBefore text);
===========================================Database script=====================================


on successfull excecution the project generates the OutputCompare.txt file 



The content of the file is as follows--->>

--------------Apk comparison Result----------------------
Old apk name=amazon-prime-video.apk
New apk name=amazon-prime-video.apk
------------------------------------
New apk package name=cm.aptoide.pt
Old apk package name=cm.aptoide.pt
------------------------------------
Old apk size=19.8MB
New apk size=19.8MB
------------------------------------
Old apk apkDexSize=6.8MB
New apk apkDexSize=6.8MB
------------------------------------
Old apk apkResourcesSize=13.3MB
New apk apkResourcesSize=13.3MB
------------------------------------
Old apk apkAssetsSize=1MB
New apk apkAssetsSize=1MB
------------------------------------
Old apk apkIsDebuggable=false
New apk apkIsDebuggable=false
------------------------------------
Old apk apkVersionInfo=versionInfo {versionCode=10050, versionName=9.18.0.2}
New apk apkVersionInfo=versionInfo {versionCode=10050, versionName=9.18.0.2}
------------------------------------
Old apk apkSdkInfo=sdkInfo {minSdkVersion=16, targetSdkVersion=25}
New apk apkSdkInfo=sdkInfo {minSdkVersion=16, targetSdkVersion=25}
------------------------------------
Old apk apkCompiledSdkVersion=28
New apk apkCompiledSdkVersion=28
------------------------------------
Old apk apkCompileSdkVersionName=9
New apk apkCompileSdkVersionName=9
------------------------------------
Old apk apkSupportedScreenSize={}
New apk apkSupportedScreenSize={}
------------------------------------
Old apk ActivityCount=37
New apk ActivityCount=37
------------------------------------
Old apk ActivityNames=[com.mopub.common.privacy.ConsentDialogActivity, com.mopub.common.MoPubBrowser, com.mopub.mobileads.MoPubActivity, com.mopub.mobileads.MraidActivity, com.mopub.mobileads.RewardedMraidActivity, com.mopub.mobileads.MraidVideoPlayerActivity, cm.aptoide.pt.view.MainActivity, com.unity3d.services.ads.adunit.AdUnitActivity, com.unity3d.services.ads.adunit.AdUnitTransparentActivity, com.unity3d.services.ads.adunit.AdUnitTransparentSoftwareActivity, com.unity3d.services.ads.adunit.AdUnitSoftwareActivity, cm.aptoide.pt.wallet.WalletInstallActivity, com.applovin.adview.AppLovinInterstitialActivity, com.applovin.adview.AppLovinConfirmationActivity, com.inmobi.rendering.InMobiAdActivity, cm.aptoide.pt.account.view.LoginActivity, com.facebook.FacebookActivity, com.facebook.CustomTabActivity, cm.aptoide.pt.DeepLinkIntentReceiver, com.smaato.soma.interstitial.InterstitialActivity, com.smaato.soma.ExpandedBannerActivity, com.fyber.inneractive.sdk.activities.InneractiveInternalBrowserActivity, com.fyber.inneractive.sdk.activities.InneractiveFullscreenAdActivity, com.fyber.inneractive.sdk.activities.InneractiveRichMediaVideoPlayerActivityCore, cm.aptoide.aptoideviews.base.MockActivity, com.facebook.CustomTabMainActivity, com.vungle.warren.ui.VungleActivity, com.vungle.warren.ui.VungleFlexViewActivity, com.vungle.warren.ui.VungleWebViewActivity, com.google.android.gms.auth.api.signin.internal.SignInHubActivity, com.google.android.gms.common.api.GoogleApiActivity, com.google.android.gms.ads.AdActivity, com.appnext.ads.interstitial.InterstitialActivity, com.appnext.ads.fullscreen.FullscreenActivity, com.appnext.banners.BannerActivity, com.appnext.core.ResultActivity, com.appnext.core.result.ResultPageActivity]
New apk ActivityNames=[com.mopub.common.privacy.ConsentDialogActivity, com.mopub.common.MoPubBrowser, com.mopub.mobileads.MoPubActivity, com.mopub.mobileads.MraidActivity, com.mopub.mobileads.RewardedMraidActivity, com.mopub.mobileads.MraidVideoPlayerActivity, cm.aptoide.pt.view.MainActivity, com.unity3d.services.ads.adunit.AdUnitActivity, com.unity3d.services.ads.adunit.AdUnitTransparentActivity, com.unity3d.services.ads.adunit.AdUnitTransparentSoftwareActivity, com.unity3d.services.ads.adunit.AdUnitSoftwareActivity, cm.aptoide.pt.wallet.WalletInstallActivity, com.applovin.adview.AppLovinInterstitialActivity, com.applovin.adview.AppLovinConfirmationActivity, com.inmobi.rendering.InMobiAdActivity, cm.aptoide.pt.account.view.LoginActivity, com.facebook.FacebookActivity, com.facebook.CustomTabActivity, cm.aptoide.pt.DeepLinkIntentReceiver, com.smaato.soma.interstitial.InterstitialActivity, com.smaato.soma.ExpandedBannerActivity, com.fyber.inneractive.sdk.activities.InneractiveInternalBrowserActivity, com.fyber.inneractive.sdk.activities.InneractiveFullscreenAdActivity, com.fyber.inneractive.sdk.activities.InneractiveRichMediaVideoPlayerActivityCore, cm.aptoide.aptoideviews.base.MockActivity, com.facebook.CustomTabMainActivity, com.vungle.warren.ui.VungleActivity, com.vungle.warren.ui.VungleFlexViewActivity, com.vungle.warren.ui.VungleWebViewActivity, com.google.android.gms.auth.api.signin.internal.SignInHubActivity, com.google.android.gms.common.api.GoogleApiActivity, com.google.android.gms.ads.AdActivity, com.appnext.ads.interstitial.InterstitialActivity, com.appnext.ads.fullscreen.FullscreenActivity, com.appnext.banners.BannerActivity, com.appnext.core.ResultActivity, com.appnext.core.result.ResultPageActivity]
------------------------------------
Old apk PermissionCount=19
New apk PermissionCount=19
------------------------------------
Old apk PermissionName=[android.permission.WAKE_LOCK, android.permission.READ_SYNC_STATS, com.android.launcher.permission.INSTALL_SHORTCUT, android.permission.RECEIVE_BOOT_COMPLETED, android.permission.INSTALL_PACKAGES, android.permission.CHANGE_WIFI_MULTICAST_STATE, android.permission.ACCESS_WIFI_STATE, android.permission.READ_SYNC_SETTINGS, android.permission.WRITE_SYNC_SETTINGS, android.permission.AUTHENTICATE_ACCOUNTS, android.permission.GET_ACCOUNTS, android.permission.MANAGE_ACCOUNTS, android.permission.INTERNET, android.permission.USE_CREDENTIALS, android.permission.READ_EXTERNAL_STORAGE, android.permission.WRITE_EXTERNAL_STORAGE, android.permission.CAMERA, android.permission.ACCESS_NETWORK_STATE, com.google.android.finsky.permission.BIND_GET_INSTALL_REFERRER_SERVICE]
New apk PermissionName=[android.permission.WAKE_LOCK, android.permission.READ_SYNC_STATS, com.android.launcher.permission.INSTALL_SHORTCUT, android.permission.RECEIVE_BOOT_COMPLETED, android.permission.INSTALL_PACKAGES, android.permission.CHANGE_WIFI_MULTICAST_STATE, android.permission.ACCESS_WIFI_STATE, android.permission.READ_SYNC_SETTINGS, android.permission.WRITE_SYNC_SETTINGS, android.permission.AUTHENTICATE_ACCOUNTS, android.permission.GET_ACCOUNTS, android.permission.MANAGE_ACCOUNTS, android.permission.INTERNET, android.permission.USE_CREDENTIALS, android.permission.READ_EXTERNAL_STORAGE, android.permission.WRITE_EXTERNAL_STORAGE, android.permission.CAMERA, android.permission.ACCESS_NETWORK_STATE, com.google.android.finsky.permission.BIND_GET_INSTALL_REFERRER_SERVICE]
------------------------------------
Old apk ServiceCount=13
New apk ServiceCount=13
------------------------------------
Old apk ServiceNames=[cm.aptoide.pt.account.AccountAuthenticatorService, cm.aptoide.pt.notification.PullingContentService, cm.aptoide.pt.install.DownloadService, cm.aptoide.pt.install.InstalledIntentService, com.google.android.gms.auth.api.signin.RevocationBoundService, androidx.work.impl.background.systemalarm.SystemAlarmService, androidx.work.impl.background.systemjob.SystemJobService, androidx.room.MultiInstanceInvalidationService, com.liulishuo.filedownloader.services.FileDownloadService$SharedMainProcessService, com.liulishuo.filedownloader.services.FileDownloadService$SeparateProcessService, com.appnext.core.AdsService, com.appnext.base.services.OperationService, com.appnext.base.services.OperationJobService]
New apk ServiceNames=[cm.aptoide.pt.account.AccountAuthenticatorService, cm.aptoide.pt.notification.PullingContentService, cm.aptoide.pt.install.DownloadService, cm.aptoide.pt.install.InstalledIntentService, com.google.android.gms.auth.api.signin.RevocationBoundService, androidx.work.impl.background.systemalarm.SystemAlarmService, androidx.work.impl.background.systemjob.SystemJobService, androidx.room.MultiInstanceInvalidationService, com.liulishuo.filedownloader.services.FileDownloadService$SharedMainProcessService, com.liulishuo.filedownloader.services.FileDownloadService$SeparateProcessService, com.appnext.core.AdsService, com.appnext.base.services.OperationService, com.appnext.base.services.OperationJobService]
------------------------------------
Old apk BroadCastCount=19
New apk BroadCastCount=19
------------------------------------
Old apk BroadCastNames=[cm.aptoide.pt.install.InstalledBroadcastReceiver, cm.aptoide.pt.notification.NotificationReceiver, cm.aptoide.pt.link.CustomTabNativeReceiver, cm.aptoide.pt.install.CheckRootOnBoot, cm.aptoide.pt.install.RootInstallNotificationEventReceiver, cm.aptoide.pt.widget.SearchWidgetProvider, com.fyber.inneractive.sdk.nativead.IANativeKit, com.fyber.inneractive.sdk.mraid.IAMraidKit, com.fyber.inneractive.sdk.video.IAVideoKit, com.facebook.CurrentAccessTokenExpirationBroadcastReceiver, com.vungle.warren.NetworkStateReceiver, androidx.work.impl.utils.ForceStopRunnable$BroadcastReceiver, androidx.work.impl.background.systemalarm.ConstraintProxy$BatteryChargingProxy, androidx.work.impl.background.systemalarm.ConstraintProxy$BatteryNotLowProxy, androidx.work.impl.background.systemalarm.ConstraintProxy$StorageNotLowProxy, androidx.work.impl.background.systemalarm.ConstraintProxy$NetworkStateProxy, androidx.work.impl.background.systemalarm.RescheduleReceiver, androidx.work.impl.background.systemalarm.ConstraintProxyUpdateReceiver, com.appnext.base.receivers.AppnextBootReciever]
New apk BroadCastNames=[cm.aptoide.pt.install.InstalledBroadcastReceiver, cm.aptoide.pt.notification.NotificationReceiver, cm.aptoide.pt.link.CustomTabNativeReceiver, cm.aptoide.pt.install.CheckRootOnBoot, cm.aptoide.pt.install.RootInstallNotificationEventReceiver, cm.aptoide.pt.widget.SearchWidgetProvider, com.fyber.inneractive.sdk.nativead.IANativeKit, com.fyber.inneractive.sdk.mraid.IAMraidKit, com.fyber.inneractive.sdk.video.IAVideoKit, com.facebook.CurrentAccessTokenExpirationBroadcastReceiver, com.vungle.warren.NetworkStateReceiver, androidx.work.impl.utils.ForceStopRunnable$BroadcastReceiver, androidx.work.impl.background.systemalarm.ConstraintProxy$BatteryChargingProxy, androidx.work.impl.background.systemalarm.ConstraintProxy$BatteryNotLowProxy, androidx.work.impl.background.systemalarm.ConstraintProxy$StorageNotLowProxy, androidx.work.impl.background.systemalarm.ConstraintProxy$NetworkStateProxy, androidx.work.impl.background.systemalarm.RescheduleReceiver, androidx.work.impl.background.systemalarm.ConstraintProxyUpdateReceiver, com.appnext.base.receivers.AppnextBootReciever]
------------------------------------
Old apk ContentProvidersCount=6
New apk ContentProvidersCount=6
------------------------------------
Old apk ContentProvidersNames=[cm.aptoide.pt.StubProvider, cm.aptoide.pt.provider, cm.aptoide.pt.FacebookInitProvider, cm.aptoide.pt.mobileadsinitprovider, cm.aptoide.pt.lifecycle-process, cm.aptoide.pt.FlurryContentProvider]
New apk ContentProvidersNames=[cm.aptoide.pt.StubProvider, cm.aptoide.pt.provider, cm.aptoide.pt.FacebookInitProvider, cm.aptoide.pt.mobileadsinitprovider, cm.aptoide.pt.lifecycle-process, cm.aptoide.pt.FlurryContentProvider]
------------------------------------
Old apk FeaturePermissionCount=1
New apk FeaturePermissionCount=1
------------------------------------
Old apk FeaturePermissionName=[android.hardware.camera]
New apk FeaturePermissionName=[android.hardware.camera]
------------------------------------
Old apk apkSignInfoMD5=99:BD:18:72:BC:56:B4:B2:61:9E:73:1A:E9:CB:DC:6F
New apk apkSignInfoMD5=99:BD:18:72:BC:56:B4:B2:61:9E:73:1A:E9:CB:DC:6F
------------------------------------
Old apk apkSignInfoSHA1=D5:90:A7:D7:92:FD:03:31:54:2D:99:FA:F9:99:76:41:79:07:73:A9
New apk apkSignInfoSHA1=D5:90:A7:D7:92:FD:03:31:54:2D:99:FA:F9:99:76:41:79:07:73:A9
------------------------------------
Old apk apkSignInfoSHA256=73:53:4D:45:C1:34:5A:47:83:C7:EF:F2:CF:60:38:55:1A:B5:FD:F0:96:73:F3:2C:68:C3:B0:86:4B:AA:80:E4
New apk apkSignInfoSHA256=73:53:4D:45:C1:34:5A:47:83:C7:EF:F2:CF:60:38:55:1A:B5:FD:F0:96:73:F3:2C:68:C3:B0:86:4B:AA:80:E4
------------------------------------
Old apk apkSignInfoFacebookHash=1ZCn15L9AzFULZn6+Zl2QXkHc6k=

New apk apkSignInfoFacebookHash=1ZCn15L9AzFULZn6+Zl2QXkHc6k=

------------------------------------
Old apk apkSignInfoPublicKey=30:81:9F:30:0D:06:09:2A:86:48:86:F7:0D:01:01:01:05:00:03:81:8D:00:30:81:89:02:81:81:00:81:2E:F3:2F:41:2D:62:0C:63:6A:89:C6:7B:BE:62:5B:4B:4D:B7:97:F4:7C:9B:35:87:94:AC:E9:78:24:B9:E0:2E:BE:E4:C3:66:05:58:7B:C6:9A:5C:2F:F7:35:2E:CF:CD:FD:33:04:BD:AA:ED:13:B1:E1:6E:A4:34:0B:DE:60:67:AB:1B:EB:85:AB:B8:07:A7:D0:5C:95:F3:B9:A5:8A:7E:17:23:5A:9D:2B:0F:54:96:E5:AA:7B:88:A0:F9:BC:70:FB:13:85:30:66:BE:73:5A:58:07:F6:DD:12:9B:37:6B:56:1D:A4:D4:1E:06:CD:2E:2D:94:D9:FE:C9:CC:37:02:03:01:00:01
New apk apkSignInfoPublicKey=30:81:9F:30:0D:06:09:2A:86:48:86:F7:0D:01:01:01:05:00:03:81:8D:00:30:81:89:02:81:81:00:81:2E:F3:2F:41:2D:62:0C:63:6A:89:C6:7B:BE:62:5B:4B:4D:B7:97:F4:7C:9B:35:87:94:AC:E9:78:24:B9:E0:2E:BE:E4:C3:66:05:58:7B:C6:9A:5C:2F:F7:35:2E:CF:CD:FD:33:04:BD:AA:ED:13:B1:E1:6E:A4:34:0B:DE:60:67:AB:1B:EB:85:AB:B8:07:A7:D0:5C:95:F3:B9:A5:8A:7E:17:23:5A:9D:2B:0F:54:96:E5:AA:7B:88:A0:F9:BC:70:FB:13:85:30:66:BE:73:5A:58:07:F6:DD:12:9B:37:6B:56:1D:A4:D4:1E:06:CD:2E:2D:94:D9:FE:C9:CC:37:02:03:01:00:01
------------------------------------
Old apk apkSignInfoVersion=3
New apk apkSignInfoVersion=3
------------------------------------
Old apk apkSignInfoSignature=2E:DE:CD:0D:01:54:BC:EA:FD:16:DF:23:DB:32:06:60:81:BC:08:46:0B:A5:E2:99:A2:94:D1:73:CC:64:29:92:74:D3:9B:09:7F:31:37:7C:94:C4:3A:0C:05:F2:21:D5:FF:BD:D6:7A:3A:09:A8:ED:6B:C7:5A:23:2D:9E:C2:1A:22:92:F9:7D:E1:82:3B:7D:21:4E:A0:1B:E8:65:F2:FA:67:10:1B:94:25:B8:74:F4:B4:4F:EB:66:96:EC:BE:05:15:19:3A:08:04:EB:9C:C7:E7:A3:79:FF:A2:4D:2A:36:2B:FB:2A:1A:20:50:F7:EE:24:E3:26:72:C5:1C:47:58
New apk apkSignInfoSignature=2E:DE:CD:0D:01:54:BC:EA:FD:16:DF:23:DB:32:06:60:81:BC:08:46:0B:A5:E2:99:A2:94:D1:73:CC:64:29:92:74:D3:9B:09:7F:31:37:7C:94:C4:3A:0C:05:F2:21:D5:FF:BD:D6:7A:3A:09:A8:ED:6B:C7:5A:23:2D:9E:C2:1A:22:92:F9:7D:E1:82:3B:7D:21:4E:A0:1B:E8:65:F2:FA:67:10:1B:94:25:B8:74:F4:B4:4F:EB:66:96:EC:BE:05:15:19:3A:08:04:EB:9C:C7:E7:A3:79:FF:A2:4D:2A:36:2B:FB:2A:1A:20:50:F7:EE:24:E3:26:72:C5:1C:47:58
------------------------------------
Old apk apkSignInfoSignAlgName=SHA1withRSA
New apk apkSignInfoSignAlgName=SHA1withRSA
------------------------------------
Old apk apkSignInfoSerialNumber=1253631231
New apk apkSignInfoSerialNumber=1253631231
------------------------------------
Old apk apkSignInfoIssuerNameDn=ST=Portugal
SubjectName : ST=Portugal
New apk apkSignInfoIssuerNameDn=ST=Portugal
SubjectName : ST=Portugal
------------------------------------
Old apk apkSignInfoSubjectNameDn=ST=Portugal
SubjectName : ST=Portugal
New apk apkSignInfoSubjectNameDn=ST=Portugal
SubjectName : ST=Portugal
------------------------------------
Old apk apkSignInfoGetNotAfter=ST=Portugal
SubjectName : ST=Portugal
New apk apkSignInfoGetNotAfter=ST=Portugal
SubjectName : ST=Portugal
------------------------------------
Old apk apkSignInfoGetNotAfter=Sat Sep 16 20:23:51 IST 2034
New apk apkSignInfoGetNotAfter=Sat Sep 16 20:23:51 IST 2034
------------------------------------
Old apk apkSignInfoGetNotBefore=Tue Sep 22 20:23:51 IST 2009
New apk apkSignInfoGetNotBefore=Tue Sep 22 20:23:51 IST 2009
------------------------------------
