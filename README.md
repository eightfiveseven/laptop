Laptop
======

Laptop is a script to set up linux servers and laptops with a Rails environment. It was forked from the Thoughtbot script of the same name after they dropped linux support.

This script is useful for server deployments as well so I've created seperate versions for those environments.

linux == A generic linux laptop. It can feasibly have the text editing software added back and allow the database to exist on the same machine.

development_server == Remove text editing and allow the database to exist on the same machine.

production_server == No text editing or database.

I get that puppet or chef is a more accepted way of automating this. :)

Requirements
------------

We support:

Ubuntu 14

Ubuntu 15

Install
-------

Install zsh and make it your default shell

chmod +x ./linux
./linux

Debugging
---------

Your last Laptop run will be saved to `~/laptop.log`. Read through it to see if
you can debug the issue yourself.

What it sets up
---------------

* [Bundler] for managing Ruby libraries
* [Exuberant Ctags] for indexing files for vim tab completion
* [Foreman] for serving Rails apps locally
* [gh] for interacting with the GitHub API
* [Heroku Config] for local `ENV` variables
* [ImageMagick] for cropping and resizing images
* [Node.js] and [NPM], for running apps and installing JavaScript packages
* [NVM] for managing versions of Node.js
* [Parity] for development, staging, and production parity
* [Rails] gem for writing web applications
* [Rbenv] for managing versions of Ruby
* [Ruby Build] for installing Rubies
* [Ruby] stable for writing general-purpose code
* [Watch] for periodically executing a program and displaying the output

[Bundler]: http://bundler.io/
[Exuberant Ctags]: http://ctags.sourceforge.net/
[Foreman]: https://github.com/ddollar/foreman
[gh]: https://github.com/jingweno/gh
[ImageMagick]: http://www.imagemagick.org/
[Node.js]: http://nodejs.org/
[NPM]: https://www.npmjs.org/
[NVM]: https://github.com/creationix/nvm
[Parity]: https://github.com/croaky/parity
[Rails]: http://rubyonrails.org/
[Rbenv]: https://github.com/sstephenson/rbenv
[Redis]: http://redis.io/
[Ruby Build]: https://github.com/sstephenson/ruby-build
[Ruby]: https://www.ruby-lang.org/en/
[Tmux]: http://tmux.sourceforge.net/
[Watch]: http://linux.die.net/man/1/watch
[Zsh]: http://www.zsh.org/

It should take less than 15 minutes to install (depends on your machine).

Laptop can be run multiple times on the same machine safely. It will upgrade
already installed packages and install and activate a new version of ruby (if
one is available).

Make your own customizations
----------------------------


Credits
-------
Thoughtbot created the original version of the linux script but has abandoned support of it.
![thoughtbot](http://thoughtbot.com/assets/tm/logo.png)


Contributing
------------

Edit the `linux` file.

License
-------

It is free software, and may be redistributed under the terms specified in the LICENSE file.
