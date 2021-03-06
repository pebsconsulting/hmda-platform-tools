## File Format Verification Tool

The [File Format Verification Tool](https://cfpb.github.io/hmda-platform-tools/file-format-verification/) is an electronic file format verification tool for filers who wish to confirm that a LAR is formatted in the required pipe delimited text file format. This verification tool will be available on a webpage that runs independently from the HMDA Platform and provides a convenient test mechanism for filers.

### Setup

Clone the repo, then from the project root directory:

```
yarn
yarn run file-format-verification
cd file-format-verification
docker run -it -p "3000:80" -v "$(pwd)/dist:/usr/share/nginx/html" nginx:1.12
```

Visit your site at your docker host IP at the above mapped port (eg `192.168.99.100:3000`)
