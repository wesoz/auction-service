# Codingly.io: Base Serverless Framework Template

https://codingly.io

## What's included
* Folder structure used consistently across our projects.
* [serverless-pseudo-parameters plugin](https://www.npmjs.com/package/serverless-pseudo-parameters): Allows you to take advantage of CloudFormation Pseudo Parameters.
* [serverless-bundle plugin](https://www.npmjs.com/package/serverless-pseudo-parameters): Bundler based on the serverless-webpack plugin - requires zero configuration and fully compatible with ES6/ES7 features.

## Getting started
```
sls create --name YOUR_PROJECT_NAME --template-url https://github.com/codingly-io/sls-base
cd YOUR_PROJECT_NAME
npm install
```

You are ready to go!

## Deploy

Run the command below to deploy the entire project

```
sls deploy --verbose
```

If only the javascript has been changed, just deploy the function

```
sls deploy -f FUNCTION_NAME --verbose
```

## Invoke functions

To invoke a function to test the output, just run the command below with the parameter -l to print logs

```
sls invoke -f FUNCTION_NAME -l
```

If a function is invoked automaticaly by a schedule, you can see the outputs in the logs

```
sls logs -f FUNCTION_NAME
```

