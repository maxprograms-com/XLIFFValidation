# XLIFFValidation

 Web-based XLIFF validation writen in Java and TypeScript

## XLIFF Validation Service

You can validate your XLIFF files at [https://dev.maxprograms.com/Validation/](https://dev.maxprograms.com/Validation/)

## Requirements

- JDK 21  is required for compiling and building. Get it from [Adoptium](https://adoptium.net/).
- Gradle 9.5 or newer is required for building. Get it from [https://gradle.org/](https://gradle.org/)
- Node.js 24.15.0 LTS or newer. Get it from [https://nodejs.org/](https://nodejs.org/)

## Building

- Checkout this repository.
- Point your `JAVA_HOME` environment variable to JDK 21
- Run `npm install` to download and install NodeJS dependencies
- Run `gradle` to compile the Java code and generate `Validation.war`

## Deploying

- Configure an instance of [Apache Tomcat 9.x](https://tomcat.apache.org) to run in secure mode, with HTTPS protocol
- Copy `validation.war` to Tomcat's `webapps` folder
- Set `XLIFF_HOME` environment variable, pointing to a folder in your server
- Set `OpenXLIFF_HOME` environment variable and point it to the same folder
- Copy `catalog` folder to `XLIFF_HOME/catalog`
- Start Tomcat
- Visit `https://yourServerURL/Validation` to access the validation service

---

## Legal

License information for all included components is available in the [licenses](licenses/README.md) directory.
