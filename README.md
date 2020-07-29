# Chrome extension upload

This action uploads the specified ziped chrome extension to the provided app id.
It uses the specified refresh token to generate an access token for uploading.

## Inputs

### `client-id`

Your tokens client id

### `client-secret`

Your tokens client secret

### `refresh-token`

Google developer refresh token

### `app-id`

The target extension id.

### `file-name`

The target zipped file name.

### `publish`

Publish or not after upload (true / false)

### `target`

Publish target. 'default' or 'trustedTesters'

## Outputs

## Example usage

```
uses: Airfordable/chrome-extension-upload-action@$VERSION
with:
  refresh-token: 'xxxxxxxxxxxxxxxxxxxxxx'
  client-id: 'xxxxxxxxxxxxx'
  client-secret: 'xxxxxxxxxxxx'
  file-name: './extension.zip'
  app-id: 'xzc12xzc21cx23'
  publish: true
  target: trustedTesters
```
