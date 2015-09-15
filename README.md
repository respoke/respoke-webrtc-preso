#Getting Started with WebRTC and Respoke

Example source code from the *Getting Started with WebRTC and Respoke* Presentation. Keep in mind these samples have been written with simplicity in mind for the purpose of presentation and experimentation. As such, error handling and other common coding practices have been intentionlly left out. There are methods and events available to handle errors and other such cases, and more information can be found in the [Respoke Docs](https://docs.respoke.io).

Documentation for Respoke can be found at: https://docs.respoke.io

A copy of the presentation can be found at: https://respoke.github.io/respoke-webrtc-preso/webrtc-respoke.pdf


##connect.html
A simple example demonstrating how to create a Respoke [Client](https://docs.respoke.io/js-library/respoke.Client.html) object, and how to connect to Respoke.

[Try connect example live!](https://respoke.github.io/respoke-webrtc-preso/connect.html)


##messaging.html
Building upon the connect example, this sample illustrates how to obtain reference and send a message to another endpoint using the [getEndpoint](https://docs.respoke.io/js-library/respoke.Client.html#getEndpoint) and [sendMessage](https://docs.respoke.io/js-library/respoke.Client.html#sendMessage) methods of the Respoke [Client](https://docs.respoke.io/js-library/respoke.Client.html) object.

[Try messaging example live!](https://respoke.github.io/respoke-webrtc-preso/messaging.html)

##group-messaging.html
We already learned how to send messages to a single user in the messaging demo, so let's take this a step further and look at how to send messges to an entire group. We'll first have to join the group using the [Client.join](https://docs.respoke.io/js-library/respoke.Client.html#join) method, then we can send messages to everyone in the group using the [sendMessage](https://docs.respoke.io/js-library/respoke.Client.html#sendMessage) method of the [Group](https://docs.respoke.io/js-library/respoke.Group.html) object.

[Try group messaging example live!](https://respoke.github.io/respoke-webrtc-preso/group-messaging.html)

##video.html
Continuing down our path to awesomeness, this sample shows just how simple it is to establish an Audio and Video call using Respoke! Building upon the connection code from connect.html, we add a few `<div>` tags to house the video elements that get returned by Respoke, and use the [startVideoCall](https://docs.respoke.io/js-library/respoke.Endpoint.html#startVideoCall) method of the [endpoint](https://docs.respoke.io/js-library/respoke.Endpoint.html) object.

[Try video example live!](https://respoke.github.io/respoke-webrtc-preso/video.html)

##screensharing.html
Just like we make a video call using the [startVideoCall](https://docs.respoke.io/js-library/respoke.Endpoint.html#startVideoCall) method, we can start a screenshare using the [startScreenShare](https://docs.respoke.io/js-library/respoke.Endpoint.html#startScreenShare) of the [endpoint](https://docs.respoke.io/js-library/respoke.Endpoint.html) object.

[Try screensharing example live!](https://respoke.github.io/respoke-webrtc-preso/screensharing.html)

##style.css
Some basic CSS styles to make things just a bit more perty...
