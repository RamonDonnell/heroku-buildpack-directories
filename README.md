# heroku-buildpack-directories

Run different buildpacks against different directories 

## Usage

    $ heroku config:add BUILDPACK_URL=https://github.com/RamonDonnell/heroku-buildpack-directories.git

    $ cat .buildDirectories
    root:https://github.com/heroku/heroku-buildpack-nodejs.git#0198c71daa8
    proxy:https://github.com/heroku/heroku-buildpack-nodejs.git
    client:https://github.com/appstack/heroku-buildpack-nodejs-gulp
    worker1:https://github.com/heroku/heroku-buildpack-java
    worker2:https://github.com/heroku/heroku-buildpack-clojure
    root:https://github.com/heroku/heroku-buildpack-gradle

* _root_  will run on the root git directory
* Different buildbacks can be run on the same directory


## Credits

Copied and modified from https://github.com/ddollar/heroku-buildpack-multi