# Welcome to your CDK CI/CD Project

This is a CI/CD example project

In order to have success in your deploy you need:
- a github repository with our code in it
- be sure that your project is at root directory, use main or master for now, since it would help you on less trouble configuring branches for deployments in the pipeline stages
- an aws account ( free tier is okay )
- go to your github account -> settings -> developer settings -> personal access token -> create one classic and get the data ( don't share)
- a secrets manager key with the name github-token and the data will be stored in plain text ( remove the object default from AWS )

In the end you will have:
- a full runnable pipeline cdk deployed
- you will not need to to cdk deploy to send new resources to AWS
- do always cdk synth to check your code
- your pipeline when breaks, it will not deploy your code


## Useful commands

* `npm run build`   compile typescript to js
* `npm run watch`   watch for changes and compile
* `npm run test`    perform the jest unit tests
* `npx cdk deploy`  deploy this stack to your default AWS account/region
* `npx cdk diff`    compare deployed stack with current state
* `npx cdk synth`   emits the synthesized CloudFormation template
