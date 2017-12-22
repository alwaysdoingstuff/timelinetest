Timeline Core integration/staging tree
=====================================

[![Build Status](https://travis-ci.org/timeline/timeline.svg?branch=master)](https://travis-ci.org/timeline/timeline)

https://timelinehub.org

What is Timeline?
----------------

Timeline is an experimental digital record that enables instant token transfers to
anyone, anywhere in the world. Timeline uses peer-to-peer technology to operate
with no central authority: managing transactions and issuing tokens are carried
out collectively by the network. Timeline Core is the name of open source
software which enables the use of this technology.

All of the below assumes time-travelling backwards in the same universe or hopping across to alternate universes that exist in the same state as our past is possible.

Anyone who ever invents time-travelling needs an anchor from which to gauge changes made to the timeline, among other things I'll outline below.

TIMELINE serves as a perfect tool for time-travellers. In case you're not familiar, every 1 minute, TIMELINE creates a new block with part of the output of a previous block, plus a very special, very hard to compute number. In effect, this creates a chain (where the word blockchain records comes from) of very improbable events (finding a very special number).

If you were to time-travel effectively, one of the first things you'd need is the ability to measure and track your changes. You don't want to go back, kill Hitler, and then come back to a dystopia worse than you had before.

What TIMELINE does is make a series of permanent, distributed, unalterable points of low entropy. You can, in essence, track your timeline against a proposed timeline you're travelling to by where the blockchain records diverges. If they match, the universe must be a match. If they don't, walk backwards through the blockchain records to find the point of divergence, and there's where the change has affected the universe.

Everything in the universe affects everything else, so any change will show up in the blockchain records, but not necessarily immediately. Imagine stopping someone on the street to ask them the time. That person then goes on to do what they were going to do anyway, but they cause a chain reaction of change starting from the minute and very quickly ballooning into massive changes. Eventually, this will affect TIMELINE mining by affecting the PRNGs inside of one or more TIMELINE miners (a miner is plugged in sooner, rather than later; a user logs in at a different time, timing from electrical circuits is affected, any number of things can change), causing them to either "miss" the winning hash, or find a hash where they previously wouldn't have.

Comically, this is not so far off from the plot of Steins;Gate, which leaned heavily on the story of John Titor, a time traveller who posted for some months on an internet forum warning us that CERN would develop time-travel technology and create a dystopia. In the anime, Rintaro Okabe (the main character) receives a "divergence meter" from another time-traveller that allows him to track his changes to the timeline (either further or closer to the original point of divergence and the original timeline)

TIMELINE is also extremely useful as a permanent, eternal record of truth.

If you start recording reality into a permanent distributed ledger, when you arrive to a new reality (and you still trust mirror-you not to lie to yourself), you can just read the blockchain records to see an unalterable record of events, cryptographically proven and secure. Any information recorded into the blockchain records cannot be edited or erased without an ever-rising cost. You can disrupt information from being written (and indeed, this has happened before), but once blocks start getting stacked on top, it's essentially permanent (a lot more permanent and easier than microfiche's, that's for sure)

Which brings me to my conclusion:

EITHER Time-travel to the past or universe hopping is impossible or is never achieved by any descendants of humans (unknown possibility) OR
TIMELINE is irreparably flawed in ways we're not aware of that makes it unsuitable for a "divergence meter" and record of truth (very possible) OR
TIMELINE will be used by time-travellers to provide a point of reference for any effects they have on the planet and by their progenitors or trusted scribes to create a record of reality.
There are many companies combing the blockchain records for interesting data, and perhaps one day they'll uncover some "news feed" in the blockchain records left by an aspiring time-traveller, but in any case already there exists a technology that allows for careful, precise measurement of time-travel related activity.

TL;DR: If the universe is a spanning tree of possibilities, the blockchain records is a trail of breadcrumbs left to track one particular subset of possibilities.

I welcome any further ideas about the possible conspiratorial uses of a permanent digital record.


License
-------

Timeline Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/timeline/timeline/tags) are created
regularly to indicate new official, stable release versions of Timeline Core.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md).

The developer [mailing list](https://lists.linuxfoundation.org/mailman/listinfo/timeline-dev)
should be used to discuss complicated or controversial changes before working
on a patch set.

Developer IRC can be found on Freenode at #timeline-core-dev.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test on short notice. Please be patient and help out by testing
other people's pull requests, and remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write [unit tests](src/test/README.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`. Further details on running
and extending unit tests can be found in [/src/test/README.md](/src/test/README.md).

There are also [regression and integration tests](/test), written
in Python, that are run automatically on the build server.
These tests can be run (if the [test dependencies](/test) are installed) with: `test/functional/test_runner.py`

The Travis CI system makes sure that every pull request is built for Windows, Linux, and OS X, and that unit/sanity tests are run automatically.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.

Translations
------------

Changes to translations as well as new translations can be submitted to
[Timeline Core's Transifex page](https://www.transifex.com/projects/p/timeline/).

Translations are periodically pulled from Transifex and merged into the git repository. See the
[translation process](doc/translation_process.md) for details on how this works.

**Important**: We do not accept translation changes as GitHub pull requests because the next
pull from Transifex would automatically overwrite them again.

Translators should also subscribe to the [mailing list](https://groups.google.com/forum/#!forum/timeline-translators).
