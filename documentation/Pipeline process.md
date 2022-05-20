# Pipeline

Github Push triggers Circle Ci which tests/builds frontend/api and copy files to frontend/api S3 Buckets

Circle Ci Api build Runs the build script, exports all environment variables from CircleCI configuration to a .env file, then runs the archive script. Then uses AWS CLI to upload archive to S3.

front end deployed through S3
api deployed through elastic Beanstalk