## Video Player with Download and Play Buttons

This JavaScript code provides a simple video player with download and play buttons. It allows you to download a video and play it after downloading, ensuring that it doesn't play before downloading. Additionally, it includes some basic button styling that you can customize to match your design preferences.

### How it works

1. ### HTML Structure
   
   The HTML structure includes a video container (`videoContainer`) where the video player will be displayed, along with two buttons: "Download Video" (`downloadButton`) and "Play Video" (`playButton`). The "Play Video" button is initially hidden and becomes visible after the video is downloaded.

2. ### Download Function

   The `downloadVideo` function uses the Fetch API to download a video from a specified URL. It returns a `Blob` (Binary Large Object), which represents the binary data of the video.

3. ### Creating the Video Player

   The `createVideoPlayer` function takes a `Blob` as input and creates a video element (`videoElement`) with the following features:
   
   - It sets the `src` attribute of the video element to a URL representing the downloaded video.
   - It adds controls to the video element, allowing users to play, pause, and adjust the video's volume and playback speed.
   - It includes a "Play Video" button (`playButton`) that, when clicked, starts playing the video.
   - It includes a "Download Video" button (`downloadButton`) that allows users to download the video.

4. ### Event Listeners

   - The "Download Video" button (`downloadButton`) triggers the download process when clicked. It calls the `downloadVideo` function and then invokes `createVideoPlayer` to display the video player.
   
   - The "Play Video" button (`playButton`) becomes visible only after the video is downloaded. When clicked, it starts playing the video.
