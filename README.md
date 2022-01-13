name: Sync OAS to ReadMe
on:
  push:
    branches:
      - master
      - main
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - uses: readmeio/github-readme-sync@v2
        with:
          readme-oas-key: 1dWTFT6Jd149EGTlN6mKvlpAJbGkAA91:61e0b3c38ab7781da7c99fbd
           
          # OPTIONAL CONFIG, use if necessary
          # oas-file-path: './swagger.json'
          # api-version: 'v1.0.0'
