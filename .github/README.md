# mpg123 release snapshots

The files of the release archives of [mpg123](https://www.mpg123.de/), one commit per release, exactly as published. This is not a fork and not a mirror, and the mpg123 project does not maintain it.

mpg123 is a fast MPEG audio decoder and player. It is the work of Thomas Orgis, who maintains it and signs the releases, of its original author Michael Hipp, and of the many people credited in `AUTHORS`. It is under the LGPL 2.1 (`COPYING`). Bug reports and contributions belong to the project: https://www.mpg123.de/contact.shtml.

## Why this repository exists

[Jack Apps Collection for macOS](https://github.com/zinc75/jack-apps-collection-macos) links libmpg123 statically into its applications, and each application ships the licence and the source of what it contains. mpg123 is developed in Subversion. The Git mirror that the project points to ([madebr/mpg123](https://github.com/madebr/mpg123)) follows the development branch, and several files of the release archives are in none of its commits, so no commit of it gives the source of a release. The collection therefore needs a Git repository where the release is a commit, to reference it as a submodule. This repository keeps that copy, and it keeps the source available if a download site goes away.

## What is in it

Each tag points to a commit whose files are those of the release archive, nothing added and nothing changed. The commit message gives the address of the archive, its SHA-256 and the fingerprint of the key that signed it. The archive and its signature are also attached to the release of the same name. This `README` is the only addition: it is in `.github/`, on top of the tagged commits, and is not part of any release.
