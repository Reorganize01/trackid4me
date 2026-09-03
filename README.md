# TrackID4Me

Support files for **TrackID4Me**, a Twitch chat bot that answers `!id` with the
track currently playing in rekordbox.

This repository holds no source code. It publishes two small signed files that
the app fetches:

| File | What it is |
|---|---|
| `latest.json` | The current version, its download address and its checksum |
| `revocations.json` | Licence keys that have been withdrawn |

Both are signed with an Ed25519 key. The app checks the signature against a
public key compiled into it, so nothing here can be altered to make the app
download or trust anything the author did not sign.

Made by [Reorganize](https://www.twitch.tv/reorganize).
