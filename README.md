# ng15-build-deploy

A little node script to build and deploy corespring ng15 pie elements to a pie-catalog.

* It looks for all directories that end with `ng15`
* It removes any that have been added to a `--skip` flag
* It removes any that are found on the pie-catalog webapp (can be overridden with `--force`)
* For the remaining directories it runs `pie clean`, `pie pack ...` and then `curl ...`


## Usage

```shell 
npm install -g corespring/ng15-build-deploy
cd parent-dir/of/repos
ng15bd
```

## options

`--host` the pie catalog host default: `pie-catalog-demo.herokuapp.com`.

`--skip` skip this repo - can have multiple skip flags in the command

`--only` only run this repo - will not affect skipped repos

`--force` if the catalog already has the repo uploaded it wont deploy by default. this forces a build and deploy.