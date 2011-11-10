Requirements
------------

* [sbt](https://github.com/harrah/xsbt/wiki) 0.10.1 (does not work/compile with sbt 0.10.0) or later. NOTE: For sbt 0.7.x version of the plugin, see [branch sbt-0.7](https://github.com/mpeltonen/sbt-idea/tree/sbt-0.7)


Installation
------------

**sbt 0.10.1:**

Add the following lines to ~/.sbt/plugins/build.sbt or PROJECT_DIR/project/plugins/build.sbt

    resolvers += "sbt-idea-repo" at "http://mpeltonen.github.com/maven/"
    
    libraryDependencies += "com.github.mpeltonen" %% "sbt-idea" % "0.10.0"

**sbt 0.11.0:**

Add the following lines to ~/.sbt/plugins/build.sbt or PROJECT_DIR/project/plugins.sbt

    resolvers += "sbt-idea-repo" at "http://mpeltonen.github.com/maven/"
    
    addSbtPlugin("com.github.mpeltonen" % "sbt-idea" % "0.11.0")
    
**NOTE: If you experience problems with sbt 0.11 installation, [see this](https://github.com/mpeltonen/sbt-idea/issues/95).**

Usage
-----

Use `gen-idea` sbt task to create Idea project files.

By default, classifiers (i.e. sources and javadocs) of sbt and library dependencies are loaded if found and references added to Idea project files. If you don't want to download/reference them, use command 'gen-idea no-classifiers no-sbt-classifiers'.

Configuration settings
----------------------

TODO...

License
-------

Licensed under the New BSD License. See the LICENSE file for details.
