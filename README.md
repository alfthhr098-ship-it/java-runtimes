# java-runtimes
Java runtimes (JRE) used by the FrostDevelopment APK builder.

The APK builder downloads every file attached to the release tagged `runtime` and bundles it into the APK's `assets/components` folder:

- file names containing `jre8` or `jre-8` go to `components/jre`
- `jre17` goes to `components/jre-new`
- `jre21` goes to `components/jre-21`
- anything else goes to `components/jre-<file name>`

`.zip` files are unzipped, other files (for example `.tar.xz`) are copied as they are.
