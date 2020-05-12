# verdaccio-heroku-docker

A containerized verdaccio private npm registry.

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
