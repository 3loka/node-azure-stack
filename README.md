[![Use this template](https://github.com/stack-instance/badge.svg)](https://github.com/stack-instance?stack_template_owner=3loka&stack_template_repo=nodejs-azureapp-stack)
                  

 <p>
    <img src="https://avatars.githubusercontent.com/u/6844498?s=200&v=4" height="20">
    <b>Use this stack</b> to spin up a static website and deploy to azure in seconds.
</p>


## Why should you use this stack?
You can spin up your own Expressjs(NodeJS) website in seconds. 

Deployment happens on Azure Cloud via a Azure App Service.

The stack also sets up a proper Github CI/CD environment by taing care of the following things
1. Branch Naming convention - You can use any branch prefixed with "dev" as your development environment. 
2. Branch Protection Setting - Developers working on this branch can work freely and push changes without a PR and a code reviewer. This facilitates quick development. However the `main` Branch is setup to dismiss stale reviews
3. Enable Security alerts - A workflow will be setup for you to enable Dependabot alerts to detect vulnerabilities.
4. CodeQL Security Analysis - Discover vulnerabilities across a codebase with CodeQL, our industry-leading semantic code analysis engine

## What are the inputs to pass while setting up the stack?
```
# Name of the Azure App which has been configured to host the website
- AZURE_APP_NAME

# Azure Publish profile
- AZURE_WEBAPP_PUBLISH_PROFILE
```

#### Github apps installed with this stack
```None```

## How to setup local development server?
```
# to start a local development environment, and view in browser.
npm install
npm start
open http://localhost:3000 

# to run tests
npm test

# to generate a production build
npm build
```

## Learn more 

### ExpressJS
Visit [Expressjs.com](https://expressjs.com) to view the full documentation.

### Azure Cloud
Learn more about [Azure](https://docs.microsoft.com/en-us/azure) from the official site.


## Other Useful links

#### Security guide
Please see our guide lines for reporting issues related to [security.md](/.github/stacks/security.md).

#### Contributor guide
Please see our guide lines for [contributing.md](/.github/stacks/contributing.md).

## Contributors 
- Trilok Ramakrishna ([@3loka](https://twitter.com/3loka))
