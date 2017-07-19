# jobs.zooniverse.org
Zooniverse jobs static site

# Test locally
+ Setup node using nvm (last good: node v4.2.6, npm v2.14.12)
+ Run a local web server (http://localhost:10850) - `npm start`

# Deployment

The easy way:

* Go to https://jenkins.zooniverse.org/job/Deploy%20static/build?delay=0sec
* Select "jobs.zooniverse.org" and run it.

The hard way:

+ `npm run deploy` - https://jobs.zooniverse.org
+ `npm run stage` - https://preview.zooniverse.org/jobs/
