# salus-data-loader-content

This repo contains default data that can be populated into a deployed Salus environment.

This enables a newly deployed environment to be immedietly useful without having to populate numerous configurations manually.  For example, public monitoring zones, agent releases, or available tenants can all be populated via the use of this repo.

# Automation / Webhooks

Merges to this repo trigger the [data-loader](https://github.com/racker/salus-tools/tree/master/data-loader) webhook to be hit.  The data-loader will then run the required API requests to create any new content that has been merged.

## Branches / Environments

Merges to the following branches will trigger the webhook to run in the listed environments.

* `production` - Prod
* `staging` - Stage
* `master` - Dev, Perf

test1