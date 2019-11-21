# agora-camera-release-js

This highlights how to release the camera when muting video in an Agora integrated web application.

## Prerequisites

- A web browser

## Code Highlights

In *index.html*, pay particular attention to the streamCamera and muteCamera button click events, as well as the following Agora callbacks: 
- rtc.client.on("stream-subscribed", function (evt) {})
- rtc.client.on("stream-updated", function (evt) {})
- rtc.client.on("mute-video", function (evt) {})

## Quick Start

This section shows you how to prepare, and run the sample application.

### Obtain an App ID

To build and run the sample application, get an App ID:
1. Create a developer account at [agora.io](https://dashboard.agora.io/signin/). Once you finish the signup process, you will be redirected to the Dashboard.
2. Navigate in the Dashboard tree on the left to **Projects** > **Project List**.
3. Save the **App ID** from the Dashboard for later use.
4. Generate a temp **Access Token** (valid for 24 hours) from dashboard page with given channel name, save for later use.

### Integrate Agora Video SDK

Currently, version 2.9.0 of the Agora Web SDK is being used from Agora's hosted cdn. Alternatively, you may download the SDK, place it into **assets** directory, and rename file name as **AgoraRTCSDK-2.9.0.js** (make corresponding change in index.html).

### Run Web-Server

1. Install live-server globally via npm
    ```
    npm i live-server -g
    ```
2. Launch server via following commands in working folder,
    ```
    live-server .
    ```
3. Enter Valid APPID, Token, Channel, UID and click **Join Room**

## Resources

- You can find full API document at [Document Center](https://docs.agora.io/en/)
- You can file bugs about this demo at [issue](https://github.com/AgoraIO/Basic-Video-Call/issues)

## License

The MIT License (MIT)
