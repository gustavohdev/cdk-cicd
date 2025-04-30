# Welcome to Your CDK CI/CD Project

🛸This project demonstrates a basic CI/CD pipeline using AWS CDK. With just a few setup steps, you'll have a fully working pipeline to automate your deployments🛸

## Prerequisites

📈 To successfully deploy this project, make sure you have the following:

- A GitHub repository containing this project.
- The project must be in the root directory of the repo.
- Use `main` or `master` as the default branch for simplicity in pipeline configuration.
- An AWS account (Free Tier is sufficient).
- A GitHub Personal Access Token:
  - Go to GitHub → Settings → Developer Settings → Personal Access Tokens.
  - Create a token (classic type).
  - Copy the token (keep it private).
- An AWS Secrets Manager secret named `github-token`:
  - Store the token as plain text.
  - Remove any default `SecretObject` (just store the string value).

## What You'll Get

✅ By the end of this setup, you'll have:

- A fully working CDK pipeline deployed to AWS.
- No need to run `cdk deploy` manually—just commit and push your code.
- Use `cdk synth` regularly to validate your CDK code.
- The pipeline will not deploy your code if it breaks during any stage.

## Useful Commands

- `npm run build` – Compile TypeScript to JavaScript
- `npm run watch` – Watch for changes and auto-compile
- `npm run test` – Run Jest unit tests
- `npx cdk deploy` – Deploy the stack to your AWS account
- `npx cdk diff` – Compare deployed stack with your local changes
- `npx cdk synth` – Generate the CloudFormation template

## Tips

- Commit frequently and use small, descriptive commits to help with debugging.
- Monitor your pipeline via AWS CodePipeline for real-time feedback.
- Use `cdk destroy` to clean up your resources if needed.
