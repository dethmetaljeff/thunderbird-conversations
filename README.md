[![Build Status](https://travis-ci.org/protz/thunderbird-conversations.svg?branch=master)](https://travis-ci.org/protz/thunderbird-conversations)

Thunderbird Conversations
=========================

This extension improves the threaded summary for emails in Thunderbird. It
vastly improves the UI by including some ideas from GMail. More specifically:

* your own messages are displayed in the thread,
* you initially see summaries, they can be expanded to display full messages,
* quoted sections are collapsed à la GMail,
* fast links for replying (and possibly other useful actions),
* you can reply inline (through a "quick reply" feature).

For screenshots and a stable version, please head to
[AMO](https://addons.thunderbird.net/thunderbird/addon/gmail-conversation-view/) which should
provide you with a ready-to-install package.

Branches
========

The master branch of `thunderbird-conversations` is sometimes only compatible with the `Daily`-version of Thunderbird (sometimes it won't be, but we'll welcome pull requests to fix that). You can build this from source or get a pre-built binary at https://ftp.mozilla.org/pub/mozilla.org/thunderbird/nightly/latest-comm-central/.

Each major release typically has a release branch for that release (e.g. 2.14+). All pull requests should be against the master branch, we may transplant them after landing to the release if we want them on the release branch.

Building
========

1. Clone the repository
2. Change into the main folder, run `git submodule init` and `git submodule update`
3. Run `npm install`
4. Run `npm run build`

This will package an `.xpi` file of the latest codebase which can be installed via add-on manager in Thunderbird (hint: you can drag & drop it onto the add-on manager view).

Testing
=======

To run the tests:

```
$ npm test
```

Contributing
============

Please see [CONTRIBUTING.md](CONTRIBUTING.md).

License
=======

Please see [LICENSE](LICENSE).
