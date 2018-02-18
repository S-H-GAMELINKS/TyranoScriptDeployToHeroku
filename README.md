# TyranoScriptDeployToHeroku
## What's this ?

Deploy to Heroku for TyranoScript!

## How to use it?

At first, clone this repository.

```
git clone https://github.com/S-H-GAMELINKS/TyranoScriptDeployToHeroku.git
```

Clone is finish? you have to make a `public` directory.

```
mkdir public
```

Your Game(Made by TyranoScript or TyranoBuilder, and published Bowser Game!) put `public` directory, and commit!

```
git commit -am "Deploy to Heroku, for TyranoScript!"
```


And, Heroku App create such command. APP_NAME is your application name.

```
heroku apps:create -a APP_NAME
```

Connect to Heroku App, this command.

```
heroku git:remote -a APP_NAME
```

Push Heroku App repository.

```
git push heroku master
```

Deploy is done. Opne your Heroku App, this command.

```
heroku open -a APP_NAME
```

Enjoy TyranoSrcipt!

## ref

[HerokuにRackでdeployする(初級編:静的HTMLページ)](https://qiita.com/higuma/items/9baac9e97eeb862ef64e)
