[![Build Status](https://travis-ci.org/madhums/node-express-mongoose-demo.png)](https://travis-ci.org/madhums/node-express-mongoose-demo)

# Nodejs Express Mongoose Demo

This is a demo node.js application illustrating various features used in everyday web development, with a fine touch of best practices. The demo app is a blog application where users (signing up using facebook, twitter, github and simple registrations) can create an article, delete an article and add comments on the article.

## Boilerplate

Want to build something from scratch? use the [boilerplate app](https://github.com/madhums/node-express-mongoose)

* Checkout the [apps that are built using this approach](https://github.com/madhums/node-express-mongoose/wiki/Apps-built-using-this-approach)
* The [wiki](https://github.com/madhums/node-express-mongoose/wiki) is wip, it has some information about the way application is setup.

## Requirements

* [NodeJs](http://nodejs.org)
* [mongodb](http://mongodb.org)
* [imagemagick](http://www.imagemagick.org/script/index.php)

## Install

```sh
$ git clone git://github.com/madhums/node-express-mongoose-demo.git
$ npm install
$ cp config/imager.example.js config/imager.js
$ npm start
```

**NOTE:** Do not forget to set the facebook, twitter, google, linkedin and github `CLIENT_ID`s and `SECRET`s. In `development` env, you can simply copy
`config/env/env.example.json` to `config/env/env.json` and just replace the
values there. In production, it is not safe to keep the ids and secrets in
a file, so you need to set it up via commandline. If you are using heroku
checkout how environment variables are set [here](https://devcenter.heroku.com/articles/config-vars)

in `config/config.js`. Also if you want to use image uploads, don't forget to replace the S3 and Rackspace keys in `config/imager.js`.

Then visit [http://localhost:3000/](http://localhost:3000/)

## Tests

```sh
$ npm test
```

## License

MIT
