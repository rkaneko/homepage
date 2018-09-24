www.rkaneko.com
===

### Prerequisistes

```bash
$ pip3 install -U awscli --user
```

### Deploy

```bash
$ aws s3 sync ./public s3://${S3_BUCKET_NAME}/ \
--exclude "*.js.map" --exclude "*.css.map" \
--acl public-read \
--profile ${YOUR_PROFILE}
```
