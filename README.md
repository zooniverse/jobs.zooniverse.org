# jobs.zooniverse.org
Zooniverse jobs static site

# Test locally
+ Setup node using nvm (last good: Node 16, npm 8) - `npm ci`.
+ Run a local web server (http://localhost:3000) - `npm start`.
+ Edit the page HTML and CSS in the `build` directory.

# Deployment

Deployment is handled by Github Action. Both staging and production deployment can be run ad hoc in the actions tab as needed if you have the appropriate permissions on the repository.

## Staging

On merge to master, a Github Action is triggered to deploy to staging found at `https://jobs.preview.zooniverse.org`.

## Production

Production deployments are triggered by an update to which commit the `production-release` tag is pointed to. This tag should be updated via chat ops and then a Github Action will run that builds and uploads the files to our cloud provider found at `https://jobs.zooniverse.org/`.