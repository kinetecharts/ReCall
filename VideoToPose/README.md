In this folder, you will find a observableHQ notebook export. The original notebook is at https://observablehq.com/d/45e6162100bb65ed

This notebook takes a video served from local drive or s3, and export pose detected.

Some http servers like those from Python do not support vidvid.info call. This server will:

```
 npm install files-upload-server -g
```

Then to run:
```
cd path-of-your-video-files
files-upload-server .
```
The Kineviz-fileserver.zip contains the source code for this server.

More informaiton of the server:

### Usage:
```
files-upload-server [path] [options]
```

[path] defaults to ./upload if the folder exists, and ./ otherwise.

Now you can visit http://localhost:8008 to view your server

Available Options:
-p or --port Port to use (defaults to 8008)
-a Address to use (defaults to 0.0.0.0)
-s or --silent Suppress log messages from output
-S or --ssl Enable https.
-C or --cert Path to ssl cert file (default: cert.pem).
-K or --key Path to ssl key file (default: key.pem).
-h or --help Print this list and exit.

Paths
Access the upload files http://localhost:8008
Upload API http://localhost:8008/api/upload
Upload API (For custom dir) http://localhost:8008/api/upload?pathName=YourCustomPath
Upload examples http://localhost:8008/examples

## Development ###Install dependencies
```
yarn 
```
Run as develop Server
```
yarn dev
```
Test command
```
yarn command-test
```