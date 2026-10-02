# ouicu CLI releases

This repository only holds the released binaries of `ouicu`, the command
line tool for [ouicu](https://ouicu.com): it gives the site running on your
laptop a public address, so clients can open it on any device.

## Install

    curl -fsSL https://ouicu.com/install.sh | sh

The script picks the build for your system from the latest release here,
checks it against `checksums.txt`, and checks that file's signature with
cosign when cosign is installed. Builds are made by GitHub Actions in the
ouicu repository and signed there (Sigstore, keyless).

## Use

    ouicu login          sign in through the browser
    ouicu share 3000     https://<name>.ouicu.app -> localhost:3000
    ouicu update         install the latest release

Questions: hello@ouicu.com
