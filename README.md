My personal website and resume hosted within S3.

Nice project bro... keep it up


## Compiling css
```
sass --watch css/main.scss:css/main.css --style compressed
```

## Uploading to S3
```
aws s3 sync . s3://itsmattburgess.co.uk --exclude ".*" --exclude "*/.sass-cache/*" --storage-class=REDUCED_REDUNDANCY --sse --acl=public-read
```
