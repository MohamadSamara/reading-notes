# Read Class 34

**How are releases and versioning related?**

Releases and versioning are two important concepts in software development. A release is a specific version of a software product that is made available to users. Versioning is a system for identifying and tracking different versions of a software product.

Releases and versioning are related because releases are typically associated with specific versions of a software product. For example, a release of a software product might be called "version 1.0" or "version 2.0."

Versioning can be used to track changes to a software product over time. For example, a new release of a software product might be called "version 1.1" if it includes minor bug fixes or new features.

Versioning can also be used to distinguish between different releases of a software product that are intended for different audiences. For example, a software company might release a beta version of a new product to a select group of users before releasing a final version to the general public.

**What are the 5 main tasks you need to complete to prepare your application for release to the Google Play Store?**

The 5 main tasks you need to complete to prepare your application for release to the Google Play Store are:

1. **Configure your app for release:** At a minimum, you need to make sure that logging is disabled and removed and that your release variant has debuggable false for Groovy
2. **Build and sign a release version of your app:** You can use the Gradle build files with the release build type to build and sign a release version of your app
3. **Test the release version of your app:** Before you distribute your app, you should thoroughly test the release version on at least one target handset device and one target tablet device
4. **Update app resources for release:** Make sure that all app resources, such as multimedia files and graphics, are updated and included with your app or staged on the proper production servers.
5. **Prepare remote servers and services that your app depends on:** If your app depends on external servers or services, make sure they are secure and production ready.
