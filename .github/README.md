# mpg123 release snapshots

The files of the release archives of [mpg123](https://www.mpg123.de/), one commit per release, exactly as published. This is not a fork and not a mirror. mpg123 is developed and maintained by Thomas Orgis and its contributors at https://www.mpg123.de/: nothing is developed or maintained here, and this repository is not affiliated with the project. It only keeps snapshots of the releases.

mpg123 is a fast MPEG audio decoder and player, written originally by Michael Hipp and maintained today by Thomas Orgis, who signs the releases. The many other contributors are credited in `AUTHORS`. It is under the LGPL 2.1 (`COPYING`). Bug reports and contributions belong to the project: https://www.mpg123.de/contact.shtml.

## Why this repository exists

[Jack Apps Collection for macOS](https://github.com/zinc75/jack-apps-collection-macos) builds libmpg123 and links it statically into its applications. Each application ships the licence and the source of the libraries it contains, so the collection needs to point to the exact source of the release that it uses. It does so with a Git submodule, which needs a commit of a Git repository.

mpg123 is developed in Subversion. The Git mirror that the project itself points to ([madebr/mpg123](https://github.com/madebr/mpg123)) follows the development branch, and several files of the release archives are in none of its commits. No commit of any existing Git repository gives the source of a release. This repository fills that gap: each release is one commit, and the collection references the commit of the release it uses. The snapshots also keep the source available if the download site goes away.

## What is in it

Each tag points to a commit whose files are those of the release archive, nothing added and nothing changed. The commit message gives the address of the archive and its SHA-256 and the fingerprint of the key that signed it. The archive and its signature are also attached to the release of the same name.

The only addition is this `README`, in `.github/`, on top of the tagged commits: it is not part of any release.
