# ng15-build-deploy

A little node script to build and deploy corespring ng15 pie elements to a pie-catalog


## Usage

```shell 
npm install -g corespring/ng15-build-deploy
cd parent-dir/of/repos
ng15bd
```

## options

`--host` the pie catalog host default: `pie-catalog-demo.herokuapp.com`.

`--skip` skip this repo - can have multiple skip flags in the command

`--force` if the catalog already has the repo uploaded it wont deploy by default. this forces a build and deploy.