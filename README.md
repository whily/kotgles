scagles
=======

Scagles is a scala wrapper for Android Java binding of Open GL ES 3.1.

Features to include:

* Three.js like interface.

For more information about Scagles, please go to
  <https://github.com/whily/scagles>

Wiki pages can be found at
  <https://wiki.github.com/whily/scagles>

Development
-----------

The following tools are needed to build Scagles from source:

* JDK version 6/7 from <http://www.java.com> if Java is not available.
  Note that JDK is preinstalled on Mac OS X and available via package manager
  on many Linux systems.
* Scala (2.11.6)
* sbt (0.13.4)

To build the library, android.jar in Android SDK (the path could be
for example `$ANDROID_HOME/platforms/android-22/android.jar`)
should be copied the directory `lib/` under the source code tree.

The project follows general sbt architecture, therefore normal sbt
commands can be used to build the library: compile, doc, test,
etc. For details, please refer
<http://scala.micronauticsresearch.com/sbt/useful-sbt-commands>.

Currently the library is not published to any public repository
yet. To use this library with your project, you need to download the
source code, and run `sbt publish-local` in your command line. Then,
include following line in your sbt configuration file.

          libraryDependencies += "net.whily" %% "scagles" % "0.0.1-SNAPSHOT"
