# Cognito

The Amplify Framework uses Amazon Cognito as the main authentication provider.

## Configure Auth Category

* Execute this command `amplify add auth`:To start provisioning auth resources in the backend.
* Enter the following when prompted:

   ~~~R

    ? Do you want to use the default authentication and security configuration?
        `Default configuration`
    ? How do you want users to be able to sign in?
        `Username`
    ? Do you want to configure advanced settings?
        `No, I am done.`
  ~~~
* Execute `amplify push`:To push your changes to the cloud.
* Install Amplify Libraries
  ```
    dependencies {
         implementation 'com.amplifyframework:aws-auth-cognito:1.24.0'
     }
  ```
* Initialize Amplify Auth: Add the Auth plugin
* Check the current auth session
