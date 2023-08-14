# LambdaTest Camera Image Injection in Katalon Studio

This project demonstrates how to use LambdaTest's [Camera Image Injection][image_injection] feature with Katalon Studio. 
# Requirements

* [Katalon Studio][studio] 8.6.5 or later
* LambdaTest account with access to real devices and the Camera Image Injection feature
* An application to test that supports the Camera Image Injection feature. (This demonstration uses a sample camera app included in this repository.)

# Setting up the default profile

This demonstration expects several global variables to be set in the default profile. These variables are used to configure the application under test and the image used for testing. 

The following variables are required:

* `media_url` - The URL of the image to be injected into the application under test.
* `app_url` - The URL of the application under test. (This demonstration uses a sample camera app included in this repository.)

# Uploading the test app to LambdaTest

You can find a sample iOS camera app [SampleCameraAppLT.ipa](./SampleCameraAppLT.ipa) included in this repository. You can upload this app to LambdaTest using the [LambdaTest documentation](https://www.lambdatest.com/support/docs/upload-your-mobile-app/). Store the URL of the uploaded app in the global variable `app_url`.
# Uploading the image to LambdaTest

Follow the instructions in the [LambdaTest documentation](https://www.lambdatest.com/support/docs/camera-image-injection/) to upload an image to LambdaTest. Store the URL of the uploaded image in the global variable `media_url`.

# Configuring the Desired Capabilities for remote execution

You will need to configure the Desired Capabilities for remote execution. You can do this by editing the `Remote` execution profile. A sample JSON file [remote_caps.json](./remote_caps.json) containing desired capabilities is included in this repository. You can import this file as a starting point for configuring the desired capabilities. You will also want to fill in the Remote Server URL field with the URL of the LambdaTest Appium Grid.

# Running the demo

You can view the demonstration by following these steps:

1. Install and configure the prerequisites listed above.
2. Start Katalon Studio
3. Open this project
4. Open the test case "Capture Injected Photo"
5. Run the test case using the "Remote" execution profile

[image_injection]: https://www.lambdatest.com/support/docs/camera-image-injection/  "Camera Image Injection"
[studio]: https://katalon.com/katalon-studio  "Katalon Studio"
