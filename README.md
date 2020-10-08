# Monitor
 This is a crude, cobbled-together attempt to port the [Monitor Electron app](https://github.com/robisaacnz/monitor) to a Progressive Web App, so it can be used on Chrome OS. It doesn't work yet.
 
 The use case is to take a video and audio input from a camera or capture device, and display the video in a window while playing the audio through to the default output. In this way, you can turn your $3000 Chromebook Pixel into a $200 BVM, and (for example) play games from a nearby PlayStation through a capture device.

 <a class="buttons" href="https://github.com/robisaacnz/monitor-pwa/app.html">Try it</a>
 
## Known issues
* Resolutions higher than 1080p are not currently supported.
* Even with a good HDMI capture device, there's still 20-30ms of latency, so depending on what you want to do, this might be a problem.
* TV gamma settings are usually quite different to computer gamma settings, which can make the monitored video look dark and gloomy. There are filters that could fix this but it's highly subjective and adds more latency.
* There's no audio feedback protection because it introduces too much latency, and the system default inputs are monitored when the app first loads. Temporarily mute either your input or your output if you're using this in a noisy environment, otherwise you will make bystanders very angry.