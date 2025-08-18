# Changes relative to upstream

* uhabits-core/src/jvmMain/java/org/isoron/uhabits/core/preferences/Preferences.kt
  * Added public backup settings: storage URI, automatic backup toggle, timestamp suffix option, and backup frequency control.
* uhabits-core/src/jvmTest/java/org/isoron/uhabits/core/preferences/PreferencesTest.kt
  * Added tests covering the new public backup preferences.
* uhabits-android/src/main/java/org/isoron/uhabits/utils/DatabaseUtils.kt
  * `saveDatabaseCopy` now accepts a flag to append a date to the generated backup filename.
* uhabits-android/src/test/java/org/isoron/uhabits/utils/DatabaseUtilsTest.kt
  * Added tests for copying the database with and without a date suffix in the filename.
* uhabits-android/src/main/java/org/isoron/uhabits/database/PublicBackupWorker.kt
  * New `CoroutineWorker` that writes periodic backups to the user-selected folder and honors the date suffix preference.
* uhabits-android/src/main/java/org/isoron/uhabits/activities/settings/SettingsFragment.kt
  * Added UI for configuring public backups and scheduling of the periodic backup worker.
* uhabits-android/src/main/res/xml/preferences.xml
  * Added preference entries for public backups, including enable switch, folder picker, date suffix toggle, and frequency list.
* uhabits-android/src/main/res/values/constants.xml
  * Added constants for public backup frequency options.
* uhabits-android/src/main/res/values/strings.xml
  * Added English strings for public backup preferences and automatic backup frequency.
* uhabits-android/src/main/res/values-af-rZA/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-ar-rSA/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-bg-rBG/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-ca-rES/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-cs-rCZ/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-da-rDK/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-de-rDE/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-el-rGR/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-eo-rUY/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-es-rES/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-eu-rES/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-fa-rIR/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-fi-rFI/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-fr-rFR/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-gu-rIN/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-hi-rIN/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-hr-rHR/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-hu-rHU/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-hy-rAM/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-in-rID/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-is-rIS/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-it-rIT/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-iw-rIL/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-ja-rJP/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-ka-rGE/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-ko-rKR/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-ml-rIN/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-nl-rNL/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-no-rNO/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-pl-rPL/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-pt-rBR/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-pt-rPT/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-ro-rRO/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-ru-rRU/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-sk-rSK/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-sl-rSI/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-sr-rCS/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-sr-rSP/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-sv-rSE/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-ta-rIN/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-te-rIN/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-tr-rTR/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-ug-rCN/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-uk-rUA/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-vi-rVN/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-zh-rCN/strings.xml
  * Added translations for public backup and automatic backup options.
* uhabits-android/src/main/res/values-zh-rTW/strings.xml
  * Added translations for public backup and automatic backup options.
