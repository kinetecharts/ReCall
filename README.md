# ReCall
An experiment with AI and dance. Under construction

Use the following instructions to setup the ReCall server

2. The link https://observablehq.com/d/45e6162100bb65ed contains code for pose analysis. Download the code from this link
3. Start local http server in the root folder of the downloaded files (You can use python , npm or any other webserver)
4. Once you open the index page in a browser you should "Poses From Video Using TF-MoveNet" in the title. In that case you are done with this step
5. You will also see some errors below. These errors are due to the video not being served. You will need to set up and start the server to serve videos in the next step


## Setup Video folder
You will need to start another http server to serve videos

1. Prerequisitie : Install npm file upload ser using the following command -> npm install files-upload-server -g. You will be using the web server started by files-upload-server to server videos
2. Clone this ReCall repository
3. Go to the "VideoDownload/videos" folder (The folder contains a video named "Dance of the Sugar Plum Fairy from The Nutcracker (The Royal Ballet).mp4" that is used by the main code)
4. Start the webserver using the following command -> files-upload-server .
5. This will start the webserver to serve videos
6. Now refresh the 
7. Check the code you had downloaded from https://observablehq.com/d/45e6162100bb65ed and you should see the nutcracker video (It may take 10-15 secs to load)

## To Do:
1. Identify a list (maybe 20) solo dance videos from youtube. Use pytube to capture video streams, also grab comments and descriptions.
2. Use MoveNet https://observablehq.com/@randomfractals/tensorflow-movenet-intro to grab pose data
3. Push pose and motion (change of pose) to a VectorDB as embedding (shall we use Pinecone or Chroma?). Later on we might perform some normalization, and/or dimensionality reduction to make recall more accurate.
4. Hook up real time video to MoveNet, and run queries from VectorDB.


## Just random list of resources for now. To be cleaned up later

MoveNet: https://observablehq.com/@randomfractals/tensorflow-movenet-intro

https://www.youtube.com/watch?v=tevHCiprL8Q

https://towardsdatascience.com/how-to-auto-generate-a-summary-from-long-youtube-videos-using-ai-a2a542b6698d

https://medium.com/latinxinai/youtube-gpt-start-a-chat-with-a-video-efe92a499e60
