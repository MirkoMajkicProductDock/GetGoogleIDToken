# GetGoogleIDToken

## Use this action to get ID token from Google.

Action uses private key json file and scope as input parameters to authenticate with Google Oauth2 server.
It will return ID token which can be used to call other endpoints created on GCP. One example would be Firebase functions(Cloud run) that have authentication enabled(are not public).

## Usage

```
- name: Get Google ID Token
  id: get-id-token
  uses: MirkoMajkicProductDock/GetGoogleIDToken@v0.0.1
  with:
    private-key-file-content: ${{ secrets.KEY_FILE_CONTENT }}
    scope: ${{ secrets.SCOPE }}
```
