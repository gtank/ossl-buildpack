# OpenSSL buildpack

This builds a Heroku instance with ruby-2.0.0-p195 linked to OpenSSL 1.0.1e,
providing access to authenticated encryption modes such as GCM.

## Use with ddollar/heroku-buildpack-multi
 
    $ heroku config:set BUILDPACK_URL=https://github.com/ddollar/heroku-buildpack-multi

    $ cat .buildpacks
    https://github.com/heroku/heroku-buildpack-ruby.git
    https://github.com/gtank/ossl-buildpack.git


The binaries referenced in bin/compile were produced with Heroku anvil from the
standard sources. If you do use this, please consider hosting your own copies.
