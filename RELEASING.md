Release Process
===============

 1. Update the `CHANGELOG.md` file with relevant info and date.
 2. Update version number in `gradle.properties` file.
 3. Update version number in `hugo-example/build.gradle` file.
 4. Update version numbers in `HugoPlugin.groovy` file.
 5. Update version number in `README.md` file.
 6. Commit: `git commit -am "Prepare version X.Y.Z."`
 7. Tag: `git tag -a X.Y.Z -m "Version X.Y.Z"`
 8. Push: `git push && git push --tags`
 9. Release: `./gradlew clean assemble uploadArchives`
 10. Update version number in `gradle.properties` file to next "SNAPSHOT" version.
 11. Update version number in `hugo-example/build.gradle` file to next "SNAPSHOT" version.
 12. Update version numbers in `HugoPlugin.groovy` file to next "SNAPSHOT" version.
 13. Commit: `git commit -am "Prepare next development version."`
 14. Push: `git push`
 15. Write a script for steps 2 - 14. *(Optional)*
