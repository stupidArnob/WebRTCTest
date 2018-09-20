#### WebRTC One-to-Many video sharing in broadcasting 

=

1. This [WebRTC](https://webrtc.org/) experiment is for one-to-many transmission of audio/video streams.
2. It sets up multiple peer connections to support the multi-user connectivity feature. Rememebr, [WebRTC](https://webrtc.org/) doesn't supports 3-way handshake!
3. Multi-peers establishment opens many RTP-ports according to the number of media streamas referenced to each peer connection.
4. Multi-ports establishment causes huge [CPU and bandwidth usage](https://www.webrtc-experiment.com/docs/RTP-usage.html)!

=

If 10 users join your broadcasted room, **40 RTP ports** will be opened on your browser:

1. 10 RTP ports for **outgoing** audio streams
2. 10 RTP ports for **outgoing** video streams
3. 10 RTP ports for **incoming** audio streams
4. 10 RTP ports for **incoming** video streams

=

#### Difference between one-way broadcasting and one-to-many broadcasting

For 10 users session, in one-way broadcasting:

1. 10 RTP ports for outgoing audio stream
2. 10 RTP ports for outgoing video stream

i.e. total 20 **outgoing** RTP ports will be opened on your browser.

On each participant's side; only 2 **incoming** RTP ports will be opened.

Unlike one-way broadcasting; one-to-many broadcasting experiment opens both outgoing as well as incoming RTP ports for each participant.


#### Browser Support 

| Browser        | Support           |
| ------------- |-------------|
| Firefox | [Stable](http://www.mozilla.org/en-US/firefox/new/) / [Aurora](http://www.mozilla.org/en-US/firefox/aurora/) / [Nightly](http://nightly.mozilla.org/) |
| Google Chrome | [Stable](https://www.google.com/intl/en_uk/chrome/browser/) / [Canary](https://www.google.com/intl/en/chrome/browser/canary.html) / [Beta](https://www.google.com/intl/en/chrome/browser/beta.html) / [Dev](https://www.google.com/intl/en/chrome/browser/index.html?extra=devchannel#eula) |
| Android | [Chrome Beta](https://play.google.com/store/apps/details?id=com.chrome.beta&hl=en) |

