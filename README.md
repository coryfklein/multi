# multi

`multi` is a tool for using `git grep` on multiple repositories at once. Often at work I have multiple repositories that are interrelated and I want to grep through all of them at once. This can now be done using `multi`.

# Install

`./install`

This will install `multi` into `/usr/local/bin`. If your `$PATH` references that directory then you will be able to use `multi` from the command line immediately. Otherwise add `/usr/local/bin` to your `$PATH` first.

This will also install a `.multi` configuration file in your home directory.

# Configuration

Before using `multi` for the first time you must specify the repositories to be searched in the `REPOS` variable in your `~/.multi` file.
