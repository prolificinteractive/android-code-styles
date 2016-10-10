Android Code Styles and Quality Checks
======================================

Android Studio code style settings and code quality configs for Prolific's Android projects.


Installation for Code Styles
----------------------------

 * Run the `install.sh` script.
 * Restart Android Studio if it's running.
 * Open Android Studio Project Settings -> Code Styles, change the code style for the
   project to the one you want.

Adding Code Quality Checks to Project
-------------------------------------

 * Copy the quality folder to your project folder.
 * In your `app/build.gradle` file add the following lines whereever you define plugins:
 	- `apply from: '../quality/quality.gradle'`
    - `apply from: '../quality/jacoco/jacoco.gradle'`

 * __Run the task using `./gradlew check`__

License
-------

[![Public domain](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/legalcode)
