<template>
  <div class="hello">
  <div id="me"></div>
	<div id="remote-container"></div>
	<div id="canvas-container"></div>
	<div class="control-btns">
		<button class="exit" @click="exitStream()">Exit</button>

	</div>
  </div>
</template>

<script>
// import AgoraRTC from 'agora-rtc-sdk'

export default {
  name: 'Stream',
  props: {

  },
}  
//   data() {
//     return {
//     //   remoteContainer: document.getElementById('remote-container'),
//     //   canvasContainer: document.getElementById('canvas-container'),
//     //   client: AgoraRTC.createClient({
//     //      mode: 'live',
//     //      codec: 'h264'
//       }),
// 	},
	
//   methods: {

// addVideoStreams(streamId) {
// 	let streamDiv = document.createElement('div');
// 	streamDiv.id = streamId;
// 	streamDiv.style.transform = 'rotateY(180deg)';
// 	this.remoteContainer.appendChild(streamDiv);
// },

// removeVideoStream (evt) {
// 	let stream = evt.stream;
// 	stream.stop();
// 	let remDiv = document.getElementById(stream.getId());
// 	remDiv.parentNode.removeChild(remDiv);
// 	console.log(stream.getId());
// },

// addCanvas(streamId) {
// 	let video = document.getElementById(`video${streamId}`);
// 	let canvas = document.createElement('canvas');
// 	this.canvasContainer.appendChild(canvas);
// 	let ctx = canvas.getContext('2d');

// 	video.addEventListener('loadedmetadata', function() {
// 		canvas.width = video.videoWidth;
// 		canvas.height = video.videoHeight;
// 	}),

// 	video.addEventListener('play', function() {
// 		var $this = this;
// 		(function loop () {
// 			if(!$this.paused && !$this.ended) {
// 				if(!$this.width!==canvas.width) {
// 					canvas.width = video.videoWidth;
// 					canvas.height = video.videoHeight;
// 				}
// 				ctx.drawImage($this, 0, 0);
// 				setTimeout(loop, 1000 / 30);
// 			}
// 		})();
// 	}, 0);
// },

// initClient() {
// let client = this.client;
// client.init ('cb8aa58a151144bf9f42a2581a2f331a', () => console.log('client init')),
// client.join(null, 'agora-demo', null, (uid) => {
// 	let localStream = AgoraRTC.createStream({
// 		streamId: uid,
// 		audio: true,
// 		video: true,
// 		screen: false
// 	});
// 	localStream.init(function() {
// 		localStream.play('me');
// 		client.publish(localStream);

// 		this.client.on('stream-added', function(evt) {
// 			client.subscribe(evt.stream);
// 		});
// 		client.on('stream-subscribed', function(evt) {
// 			let stream = evt.stream;
// 			addVideoStream(stream.getId());
// 			stream.play(stream.getId());
// 			addCanvas(stream.getId());
// 		});
// 		client.on('stream-removed', removeVideoStream());
// 	});
// })
// }
//   }
// }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
