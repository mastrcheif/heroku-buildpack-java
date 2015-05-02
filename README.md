Heroku buildpack for Java with maven included

## How it works

The buildpack will detect your app as Java if it has a `pom.xml` file in its root directory.  It will use Maven to execute the build defined by your `pom.xml` and download your dependencies. The `.m2` folder (local maven repository) will be cached between builds for faster dependency resolution. The mvn executable or the .m2 folder will be available in your slug at runtime.


License
-------

Licensed under the MIT License. See LICENSE file.
