# :fire: Awesome express boilerplate using authentication with Google
This is a basic and awesome express boilerplate for use authentication with Google in your applications.

## Requirements
- [App google](https://console.developers.google.com/) with **google+ api enabled** and **OAuth client ID** credentials

- [Mongo database](https://mlab.com)


## Instalation

```
git clone https://github.com/felansu/boilerplate-express-oauth-google

cd boilerplate-express-oauth-google

npm install
```

For **development environment** you need create `dev.js` file in **config** folder:
```
module.exports = {
  googleClientID: 'YOUR_GOOGLE_CLIENT_ID',
  googleClientSecret: 'YOUR_CLIENT_SECRET',
  mongoURI: 'YOUR_MONGO_URI',
  cookieKey: 'YOUR_COOKIE_KEY' (for example: anythingasdfadssfdf)
};
```

and *production environment* you need create `prod.js` file in **config** folder:
```
module.exports = {
  googleClientID: process.env.GOOGLE_CLIENT_ID,
  googleClientSecret: process.env.GOOGLE_CLIENT_SECRET,
  mongoURI: process.env.MONGO_URI,
  cookieKey: process.env.COOKIE_KEY
};
```

In production environment case you will need add this environments keys in your server production. In the example i'm using [Heroku](https://www.heroku.com) but you can use anything.
