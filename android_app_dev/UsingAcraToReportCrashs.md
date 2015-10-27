# Using Acra To Report Crashes

## Backend to Receiver Reports

* Install acralyzer in smileupps.com. 
* Create Report User and get ACRA configuration params. Note: formKey=""

## Integrated into Android Application

* Add `compile 'ch.arca:arca:4.5.+` in gradle. Note: 4.7.0 depends on android-annoation:23.0.1, conflict with com.android.support.test:runner:0.3.
* Add `@ReportCrashs` in Application.
* Add `ACRA.init(this)` in Application's `onCreate()` method.

Then acra should work now.
