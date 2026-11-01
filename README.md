# Pixel4dev.downloader - releases

This repo hosts only the **built, signed installer files** and the `update.json` manifest that
Pixel4dev.downloader's in-app updater checks. It contains no source code - see
[pixel4dev-downloader](https://github.com/buzzxstory/pixel4dev-downloader) (private) for that.

`update.json` is read by the app from:
`https://raw.githubusercontent.com/buzzxstory/pixel4dev-downloader-releases/main/update.json`

Every installer's SHA-256 in `update.json` is verified by the app before it runs it - this repo
being public and unauthenticated does not weaken that: a tampered or substituted file simply
fails the hash check.
