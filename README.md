# verdaccio-heroku-docker

A containerized verdaccio private npm registry.

## Deployment

You can deploy to heroku with one click

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

Once the app has been deployed, you will need to setup a github oauth app and add the necessary
oauth credentials as heroku config vars.

## How to publish package
1. Run console with heroku-cli or dashboard
```
heroku run sh -a {app-name}
```
2. adduser to verdaccio
```
npm adduser --registry https://{app-name}.herokuapp.com
```
2. Publish
```
npm publish --registry https://matari-npm.herokuapp.com
```
3. Refresh this page.
