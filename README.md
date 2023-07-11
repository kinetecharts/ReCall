# ReCall
An experiment with AI and dance. Under construction

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
