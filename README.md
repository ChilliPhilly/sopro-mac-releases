# sopro-mac-releases

The update channel for the macOS build of Sopro. Releases hold only the built
app (`Sopro.app.tar.gz`) and the updater manifest (`latest.json`). The source
code is private and is not here.

Installed copies of Sopro read
`releases/latest/download/latest.json` at startup and every 6 hours. Every
update is signed, and the app refuses any file that doesn't verify against the
public key built into it.

Releases are published by `scripts/release-mac.sh` in the private repo. Don't
upload files here by hand.
