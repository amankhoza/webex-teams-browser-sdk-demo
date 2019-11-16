# Webex Teams Browser SDK Demo

## 1) Prerequisites
Ensure you have Node.js installed on your OS and that you have a valid Webex Teams access token from [developer.webex.com](https://developer.webex.com/), this can be either a bot or personal user access token.

## 2) Build and run the demo
Open a terminal, create a new directory and run the following commands:
```
git clone https://github.com/amankhoza/webex-teams-browser-sdk-demo.git
cd webex-teams-browser-sdk-demo
npm init -y
npm install --save webex
npm install --save-dev parcel-bundler
```
Now open `app.js` with your favourite editor and replace `<insert_your_access_token_here>` with your own access token.

Finally run:
```
./node_modules/.bin/parcel index.html
```

This will install the relevant node dependencies and then build and serve the demo web app.

## 3) Try the demo

Visit [localhost:1234](http://localhost:1234) in your web browser to try the demo.

The demo sets up a video call, then performs manipulation on the local video stream and provides a visualisation for the remote audio. Local and remote video frames can be captured programmatically, however for the purposes of the demo we have provided buttons that allow you to easily download the current local or remote video frames respectively.

This is just a brief demonsration of what you can do with the raw video and audio streams. For more information and inspiration lookup the html5 `<video>` `<audio>` and `<canvas>` tags, as well as the [Media Streams API](https://developer.mozilla.org/en-US/docs/Web/API/Media_Streams_API).

# Resources

[Webex Teams Browser SDK Samples](https://developer.webex.com/docs/sdks/browser/samples) | Original Single Party Call sample code taken from here. More demos can be found here.

[Mozilla Developer Guide: Audio and Video manipulation](https://developer.mozilla.org/en-US/docs/Web/Guide/Audio_and_video_manipulation) | Greyscale video manipulation code taken from here.

[Mozilla Developer Guide: Web Audio API Analyser Node](https://developer.mozilla.org/en-US/docs/Web/API/AnalyserNode) | Audio visualisation code taken from here.
