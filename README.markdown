# Brazen Dropouts Bike Swap

This is the Jekyll site which powers bdbikeswap.com.

## Contributing

One goal of using Jekyll in conjunction with GitHub is to eliminate the need for cloning this repository to perform common tasks.
However, it can be nice to run a copy of the site locally to preview changes and whatnot.
Included in this repository is a Vagrantfile which, with a few plugins, should make local development a matter of running `vagrant up`.

1. `$ git clone git@github.com:brazendropouts/bdbikeswap.com && cd bdbikeswap.com`.
1. Install [Vagrant](http://www.vagrantup.com/downloads.html)
2. Install the [vagrant-omnibus](https://github.com/schisamo/vagrant-omnibus) plugin: `vagrant plugin install vagrant-omnibus`
3. Install the [vagrant-berkshelf](https://github.com/berkshelf/vagrant-berkshelf) plugin: `vagrant plugin install vagrant-omnibus`
4. `$ vagrant up`
5. `$ bin/jekyll serve -w --force_polling`
6. Admire the site at http://localhost:4000
