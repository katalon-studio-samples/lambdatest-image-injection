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

<img width="1039" alt="Cursor_and_Katalon_Studio_-_8_6_5-f5bed021_-_LambdaTest_iOS_Mobile_Demo_-__Location___Users_coty_Code_katalon_samples_lambdatest-image-injection_" src="https://github.com/katalon-studio-samples/lambdatest-image-injection/assets/1128/62be391b-f2fd-450f-8ee5-e0ee192eaa55">

# Uploading the test app to LambdaTest

You can find a sample iOS camera app [SampleCameraAppLT.ipa](./SampleCameraAppLT.ipa) included in this repository. You can upload this app to LambdaTest using the [LambdaTest documentation](https://www.lambdatest.com/support/docs/upload-your-mobile-app/). Store the URL of the uploaded app in the global variable `app_url`.

# Uploading the image to LambdaTest

Follow the instructions in the [LambdaTest documentation](https://www.lambdatest.com/support/docs/camera-image-injection/) to upload an image to LambdaTest. Store the URL of the uploaded image in the global variable `media_url`.

<img width="314" alt="App_Testing_on_Real_Device" src="https://github.com/katalon-studio-samples/lambdatest-image-injection/assets/1128/743044a3-e783-46dd-9d49-ad51c0004c9d">

# Configuring the Desired Capabilities for remote execution

You will need to configure the Desired Capabilities for remote execution. You can do this by editing the `Remote` execution profile. A sample JSON file [remote_caps.json](./remote_caps.json) containing desired capabilities is included in this repository. You can import this file as a starting point for configuring the desired capabilities. You will also want to fill in the Remote Server URL field with the URL of the LambdaTest Appium Grid.

<img width="950" alt="Project_Settings" src="https://github.com/katalon-studio-samples/lambdatest-image-injection/assets/1128/74939330-ecab-4f7d-a604-2de96d61e61f">

# Running the demo

You can view the demonstration by following these steps:

1. Install and configure the prerequisites listed above.
2. Start Katalon Studio
3. Open this project
4. Open the test case "Capture Injected Photo"
5. Run the test case using the "Remote" execution profile

[image_injection]: https://www.lambdatest.com/support/docs/camera-image-injection/  "Camera Image Injection"
[studio]: https://katalon.com/katalon-studio  "Katalon Studio"
