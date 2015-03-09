PNWPHP Website
==============

This repository contains (almost) everything that makes up
[pnwphp.com](https://pnwphp.com).

Powered by [Sculpin](https://github.com/sculpin/sculpin). =)

Build
-----

### If You Already Have Sculpin

    sculpin install
    sculpin generate --watch --server

Your newly generated clone of [pnwphp.com](https://pnwphp.com) is now
accessible at `http://localhost:8000/`.

### If You Need Sculpin

    curl -O https://download.sculpin.io/sculpin.phar
    php sculpin.phar install
    php sculpin.phar generate --watch --server

NPM + Bower + SASS
------------------

This was setup to use NPM to install Bower locally. I am not 100% certain how to
best get SASS into the mix so I was just using SASS locally. After running
`npm install` I was able to run the following command to build the CSS:

    sass --watch sass/main.scss:source/assets/css/main.css -I .

It would probably be a good idea to get this all built into one system so
possibly getting NPM to install SASS so that it can be run locally without
having it be required to be installed globally?
