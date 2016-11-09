# Class 13 -  Production Deployment

## Class videos

## Helpful Resources

# Terminal:
```console
git clone https://github.com/heroku/node-js-getting-started.git
cd node-js-getting-started
git remote -v  // origin should point to Heroku's GitHub repo

heroku create rick-301

git remote -v // origin remains, but now we see a heroku remote as well

heroku apps
heroku apps:info
heroku apps:rename tutorial-by-rick
heroku config // Will list any current config vars
heroku config:set CONFIG_VAR=someVar
heroku config:unset CONFIG_VAR
heroku sharing:add brian@codefellows.com

git status
git push heroku master
heroku open
// make changes, then before pushing:
heroku local web
git push heroku branch:master (if pushing from a branch other than your current one)


heroku releases
heroku releases:info vNumber // ex: heroku releases:info v2
heroku rollback  // rollback one release
heroku rollback v1 // rollback to a specific release
heroku apps:destroy app-name
```
