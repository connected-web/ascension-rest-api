# Ascension REST API

This project contains the REST API for Ascension built upon AWS SAM.

## Prerequisites

To use the SAM CLI, you need the following tools:

* SAM CLI - [Install the SAM CLI](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-cli-install.html)
* NodeJS - [Install NodeJS LTS](https://nodejs.org/en/); includes the NPM package management tool.

## Getting Started

`cd api-code`

`npm install`

To run the tests

`npm test`

## Building and deploying

From the project root:

`npm run build`

`sam deploy --guided`

## Accessing the API

The API has not yet been deployed.

## Authorization

The API is protected by API Keys. In order to interact with endpoints other than the status endpoint, the following headers need to be provided:

```js
headers: {
  'ascension-user': 'User Name',
  'ascension-user-api-key': 'API KEY STRING'
}
```

To create new API keys please talk to a system administrator.

## TODO

- Create staging for Dev, QA, and Prod environments 
- Develop SimpleTable resource for User model
- Create a stable Route 53 records for the API gateway URL


