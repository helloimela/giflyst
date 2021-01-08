# giflyst-backend

Spotify API Web Auth

Forked from https://github.com/spotify/web-api-auth-examples


### How to start

1. Clone this repository

2. Install package dependencies using `npm i`

3. Make sure to register application in Spotify developer's app https://developer.spotify.com/dashboard/applications

4. Setup local environment variable for node application using [dotenv](https://www.npmjs.com/package/dotenv)

5. Set your CLIENT_ID and CLIENT_SECRET 

6. On line `108`, FRONTEND_URI should point to the server of your application. If you clone from [Giflyst frontend](https://github.com/helloimela/giflyst), you should not change anything.

7. When everything is ready, run `npm start` and it will run the backend in `http://localhost:8888/`


### Deploy to heroku

1. From your command line, create heroku app.

```shell
heroku login
heroku create app_name
```

2. Create variables in your heroku app. [This is how to do it](https://devcenter.heroku.com/articles/config-vars).

3. Add variables for :

```
SPOTIFY_CLIENT_ID
SPOTIFY_CLIENT_SECRET
REDIRECT_URI
FRONTEND_URI
```

4. To deploy to heroku, make sure you have added your application in your own git repository.

```shell

git push heroku master

```
