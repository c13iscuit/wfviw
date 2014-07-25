# WFVIW!?

_What Fucking Version is Where!?_ keeps track of what's deployed, and where.

## Running

    bundle install
    bundle exec ruby wfviw.rb

## Adding Versions

Add something like following to your deployment script/hook/whatever:

    curl -d 'environment=production&name=website&version=v0.2.1' http://localhost:4567/deploy

The following parameters are accepted

Required:

  * `environment`
  * `name`
  * `version`

Optional:

  * `hostname`
  * `deployed_by`

## Other Ways to Track Deployments

* https://github.com/mydrive/capistrano-deploytags
* https://github.com/forward/capistrano-deploy-tagger
