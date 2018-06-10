# HOW TO CREATE A WEBRTC SIGNALLING VIDEO CALL APP WITH PUSHER

WebRTC (Web Real-Time Communications) is a technology which enables Web applications and sites to capture and optionally stream audio and/or video media, and to exchange arbitrary data between browsers without requiring an intermediary. The set of standards that comprises WebRTC makes it possible to share data and perform teleconferencing peer-to-peer, without requiring that the user install plug-ins or any other third-party software. 

[View tutorial](https://pusher.com/tutorials/webrtc-video-call-app-nodejs)

## Getting Started
Clone the project repository by running the command below if you use SSH

```
git clone git@github.com:samuelayo/pusher_webrtc.git
```

If you use https, use this instead

```
git clone https://github.com/samuelayo/pusher_webrtc.git
```

Change directory into the newly cloned project and install dependencies

```
cd pusher_webrtc
npm install
```

### Prerequisites

#### Setup Pusher

If you don't have one already, create a free Pusher account at https://pusher.com/signup then login to your dashboard and create an app. 


Then fill in your Pusher app credentials in your `index.js` file by replacing this line with your appid, appkey and app secret respectively:

```
const pusher = new Pusher({
    appId: 'XXX-APP-ID',
    key: 'XXX-APP-KEY',
    secret: 'XXX-APP-SECRET',
    cluster: 'XXX-APP-CLUSTER',
    encrypted: true
});
```

Also, remember to fill in the your app key and app cluster in your `index.html` file by updating this line:

```
var pusher = new Pusher('XXX-APP-KEY', {
    cluster: 'XXX-APP-CLUSTER',
    encrypted: true,
    authEndpoint: 'pusher/auth'
});
```

And finally, start the application by running:

```
node index.js
```

Visit http://localhost:3000 in your browser to view the demo.

## Built With

* [Pusher](https://pusher.com/) - APIs to enable devs building realtime features
* [Node.js](https://nodejs.org/) - Node.js® is a JavaScript runtime built on Chrome's V8 JavaScript engine. 

