# ReCall
An experiment with AI and dance. Under construction

Use the following instructions to setup the ReCall server

1. VideoDownload folder contains a python code to download youtube video.
2. Needs a local http server to serve file
3. https://observablehq.com/d/45e6162100bb65ed contains code to to pose analysis. Download the code from here
4. Start local http server in the root folder of the downloaded files (You can use python , npm or any other webserver)


## Setup Video folder
You will need to start another http server to serve videos

1. Prerequisitie : Install npm file upload ser using the following command -> npm install files-upload-server -g
2. Clone the ReCall repository
3. Go to the "VideoDownload/videos" folder (The folder contains a video named "Dance of the Sugar Plum Fairy from The Nutcracker (The Royal Ballet).mp4" that is used by the main code)
4. Start the webserver using the following command -> http-server
5. This will start the webserver to serve vides
6. Check the code you had downloaded from https://observablehq.com/d/45e6162100bb65ed and you should see the nutcracker video (It may take 10-15 secs to load)

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
