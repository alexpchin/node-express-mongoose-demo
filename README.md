# Nodejs Express Mongoose Demo

Inspired by the work of [Madhums](https://github.com/madhums/node-express-mongoose-demo).

This is a demo node.js application illustrating various features used in everyday web development, with a fine touch of best practices. The demo app is a blog application where users (signing up using facebook, twitter, github and simple registrations) can create an article, delete an article and add comments on the article.

## Boilerplate

Want to build something from scratch? use the [boilerplate](https://github.com/madhums/node-express-mongoose)

* Checkout the [apps that are built using this approach](https://github.com/madhums/node-express-mongoose/wiki/Apps-built-using-this-approach)
* The [wiki](https://github.com/madhums/node-express-mongoose/wiki) is wip, it has some information about the way application is setup.

## Requirements

* [NodeJs](http://nodejs.org) >= 6.x 
* [mongodb](http://mongodb.org)
* ~~[imagemagick](http://www.imagemagick.org/script/index.php)~~

## Install

```sh
$ git clone git://github.com/madhums/node-express-mongoose-demo.git
$ npm install
```

**NOTE:** Do not forget to set the facebook, twitter, google, linkedin and github `CLIENT_ID`s and `SECRET`s. In `development` env, you can set the env variables by doing

```sh
cp env.example .env
```

and replace the values there. In `production` env, it is not safe to keep the ids and secrets in a file, so you need to set it up via commandline. If you are using heroku checkout how environment variables are set [here](https://devcenter.heroku.com/articles/config-vars).

If you want to use image uploads, don't forget to set these env variables for
imager config.

```sh
IMAGER_S3_KEY=AWS_S3_KEY
IMAGER_S3_SECRET=AWS_S3_SECRET
IMAGER_S3_BUCKET=AWS_S3_BUCKET
```

then

```sh
$ npm start
```

Then visit [http://localhost:3000/](http://localhost:3000/)

## Tests

```sh
$ npm test
```

## License

MIT
