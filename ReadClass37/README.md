# Read Class 37

**What is Amazon S3?**

Amazon Simple Storage Service (S3) is a scalable, object storage service offered by Amazon Web Services (AWS). It is designed for storing and retrieving any amount of data, from gigabytes to petabytes, at low costs. S3 is widely used for a variety of applications, including web hosting, data lakes, backups, and disaster recovery.

**List at least 3 features that it offers to its users:**

* **Storage classes**

* **Storage management**

* **Access management and security**

* **Data processing**

**What is an object key?**

An object key is a unique identifier for an object stored in S3. It consists of a bucket name and an object name. For example, the object key "myBucket/myImage.jpg" identifies an object named "myImage.jpg" stored in the bucket "myBucket".

**S3 with Amplify:**

Amplify is a framework from AWS that makes it easy to add AWS features to your mobile and web applications. Amplify includes a Storage category that provides a simplified interface for interacting with S3.

**Which dependencies are needed to install Amplify AWS S3 to your ndroid application?**

```dependencies
dependencies {
    implementation 'com.amplifyframework:aws-storage-s3:2.14.5'
    implementation 'com.amplifyframework:aws-auth-cognito:2.14.5'
}
```

**Uploading Data to S3 with Amplify:**

To upload to S3 from a data object, specify the key and the data object to be uploaded.

```java
private void uploadFile() {
    File exampleFile = new File(getApplicationContext().getFilesDir(), "ExampleKey");

    try {
        BufferedWriter writer = new BufferedWriter(new FileWriter(exampleFile));
        writer.append("Example file contents");
        writer.close();
    } catch (Exception exception) {
        Log.e("MyAmplifyApp", "Upload failed", exception);
    }

    Amplify.Storage.uploadFile(
            "ExampleKey",
            exampleFile,
            result -> Log.i("MyAmplifyApp", "Successfully uploaded: " + result.getKey()),
            storageFailure -> Log.e("MyAmplifyApp", "Upload failed", storageFailure)
    );
}
```

Upon successfully executing this code, you should see a new folder in your bucket, called public. It should contain a file called ExampleKey, whose contents is Example file contents.

**what method(s) initialize(s) the Amplify Auth and Storage categories?**

To initialize the Amplify Auth and Storage categories you call Amplify.addPlugin() method for each category. To complete initialization call Amplify.configure().

Add the following code to your onCreate() method in your application class:

```java
public class MyAmplifyApp extends Application {
    @Override
    public void onCreate() {
        super.onCreate();

        try {
            // Add these lines to add the AWSCognitoAuthPlugin and AWSS3StoragePlugin plugins
            Amplify.addPlugin(new AWSCognitoAuthPlugin());
            Amplify.addPlugin(new AWSS3StoragePlugin());
            Amplify.configure(getApplicationContext());

            Log.i("MyAmplifyApp", "Initialized Amplify");
        } catch (AmplifyException error) {
            Log.e("MyAmplifyApp", "Could not initialize Amplify", error);
        }
    }
}
```

Note that because the storage category requires auth, you will need to either configure guest access or sign in a user before using features in the storage category.
