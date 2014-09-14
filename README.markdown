# Brazen Dropouts Bike Swap

This is the Jekyll site which powers http://bdbikeswap.com.

## Contents

### index.html

The public-facing site with Brazen Dropouts Bike Swap information. Much of the data on the site is stored in `_config.yml` so that it can be reused in the flyer with less risk of having different information across the two.

### flyer.html

The source of the flyer PDF. This exists primarily so that someone can, with some patience, print the HTML to a PDF and distribute the PDF for hanging and whatnot. See flyer.pdf in the root directory for an example of what that looks like

### canvas.html

A canvas of sorts. We use this to lay out "images" in HTML using SVG and font elements. This makes it easy to scale up or scale down the size of the image without sacrificing image quality. To capture an image, simply take a screenshot.

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
