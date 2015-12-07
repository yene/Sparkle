# Sparkle for Github
An easy-to-use software update framework for OS X developers on Github.

![github](github.png)
![sign](sign.png)

## Differences from Sparkle
* It uses the Version instead of Build number.
* The Github version can contain a "v".
* It uses latest github release.
* Only uses code signing to check the identity, so you have to sign your binary.
* No system profile can be sent.

## Credits
* [Marked.js](https://github.com/chjj/marked) for parsing markdown.

## How to release an update
A quick guide:

1. Increase *Version* number under General
2. Commit all files
3. Push master to Github
4. In Xcode archive Version and Export a Developer ID-signed Application
5. Zip the exported application
6. On github create a new release with the same version
7. Test update

The *Build* version does not matter.

## Todo
* add nice custom github style to the changelog window
* add additional security checks for SSL
