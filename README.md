# multi

`multi` is a tool for using `git grep` on multiple repositories at once. Often at work I have multiple repositories that are interrelated and I want to grep through all of them at once. This can now be done using `multi`.

# Install

`./install`

This will install `multi` into `/usr/local/bin`. If your `$PATH` references that directory then you will be able to use `multi` from the command line immediately. Otherwise add `/usr/local/bin` to your `$PATH` first.

This will also install a `.multi` configuration file in your home directory.

# Configuration

Before using `multi` for the first time you must specify the repositories to be searched in the `REPOS` variable in your `~/.multi` file.

# Example

```bash
$ cd ~/src
$ ls
vim spring-framework gradle phantomjs
$ multi -i "fantastic"
vim
====================================================
runtime/doc/quotes.txt:VIM 4.5 is really a fantastic editor.  It has sooooo many features and more
runtime/doc/quotes.txt:fantastic it is! (Tony Nugent, Australia)
spring-framework
====================================================
gradle
====================================================
subprojects/docs/src/docs/userguide/ant.xml:        simply by relying on Groovy, and the fantastic <literal>AntBuilder</literal>.
subprojects/docs/src/docs/userguide/buildScriptsTutorial.xml:            relying on Groovy. Groovy is shipped with the fantastic <literal>AntBuilder</literal>. Using Ant tasks
subprojects/docs/src/docs/userguide/ideSupport.xml:            if you do this you have a fantastic IDE support for developing Gradle scripts. Of course if you use
phantomjs
====================================================
test/ghostdriver-test/fixtures/common/macbeth.html:<A NAME=1.3.55>Are ye fantastical, or that indeed</A><br>
test/ghostdriver-test/fixtures/common/macbeth.html:<A NAME=1.3.148>My thought, whose murder yet is but fantastical,</A><br>
