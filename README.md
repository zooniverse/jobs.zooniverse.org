# jobs.zooniverse.org
Zooniverse jobs static site

# Test locally
+ Setup node using nvm (last good: node v14.5.5, npm v6.14.11) - `npm install`
+ Run a local web server (http://localhost:1085) - `npm start`

# Deployment

Deployment is handled by Github Action. Both staging and production deployment can be run ad hoc in the actions tab as needed if you have the appropriate permissions on the repository.

## Staging

On merge to master, a Github Action is triggered to deploy to staging found at `https://preview.zooniverse.org/jobs/`.

## Production

Production deployments are triggered by an update to which commit the `production-release` tag is pointed to. This tag should be updated via chat ops and then a Github Action will run that builds and uploads the files to our cloud provider found at `https://jobs.zooniverse.org/`.