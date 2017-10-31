# mc_dory #

A very simple API for transient (TTL bound) ETS data.

All thanks go to g-andrade and his [backwater library](https://github.com/g-andrade/backwater/).
This code is extracted from its backwater_cache module.

#### Requirements

* Erlang/OTP 19 and up
* rebar3

#### Features

* A basic KV store backed by ETS
* Each key can expire after a configurable TTL
* A garbage collection process, with a configurable cadency, to periodically purge expired keys.

#### Why the name?

Dory is a very forgetful fish in the movie Nemo.

Build
-----

    $ rebar3 compile