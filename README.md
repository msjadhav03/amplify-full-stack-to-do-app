# AWS Amplify

- Solution 🖥️ for `full stack application` build, ship and deployment.
- You can think of AWS Amplify as a JavaScript library that lets you build and deploy serverless applications in the cloud. It is a full-stack application platform that combines both client-side and server-side code.

# Prerequisites 🛠️

- Node.js v14.x or above
- npm v6.14.4 or above
- git v2.14.1 or above

# AWS CLI : Need to Configure Access Key and Secrete Key of User for CLI

- `aws-cli`
  1. Command Line Tool (CLI) 👨‍💻️ to interact and manage AWS services from local
     terminal.
  2. Performs tasks like creating, configuring, and managing AWS resources.
  3. Cross Platform, Access AWS APIS, Support for MFA 🔐️, Scripting and
     Automation, Customization.
  4. Installing AWS CLI on ubuntu
  ```js
  curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
  unzip awscliv2.zip
  sudo ./aws/install
  ```
- Use below command to configure  🔧️ AWS profile. Please make sure to create and use access key for CLI.
```js
aws configure
```
Provide Access key and Secret

# Install : AWS CLI npm Package 👨‍💻️

Installing `aws-amplify` package.
```js
npm install -g @aws-amplify/cli
npm i aws-amplify
```

# Start Project: Initalizing your project. 

Use below command to initalize aws amplify 📱️ app. 
```js
amplify init
```

`Note : All below Command Suppose to run in Root Directory of Application`

# Create API : Adding API to application

Use below command to add APIs. 📩️
```js
amplify api add
```
Provide required details.

# Test API : Testing API locally

- To do Testing Locally use `mock` command. ⚔️
```js
amplify mock api
```

# Status : Checking Amplify Status

To check application status 📊️ use below command.  Command suppose to run in root directory 📂️ of application. 
```js
amplify status
```

# API Push : Making API Available 📤️

Use below command to push changes to cloud. 
```js
amplify push
```

# Configuring ⚔️ : Front end with Amplify

- Use below lines to configure amplify in Front end App. 
```js
import awsExports from "./aws-exports";
Amplify.configure(awsExports);
```

# Hosting : Adding ➕️ Hosting for Front End App

- Use below command to specify hosting method. 
```js
amplify add hosting
```
- Provide required details.

# Publish : Pushing 📤️ Front end App to use

- Use below command to push front end
```js
amplify publish
```

# Auth : Adding ➕️ Auth to application 🛡️

- `auth` 🔐️ command is used to add auth to application. Secure you app with AWS Cognito Serrvice.
```js
amplify add auth
``` 

# Deleting Amplify Application 🚮️
- Navigate 👉️ to root folder of Application and use following command.
```js
amplify delete
```

# To run this application
1. Clone ⬇️ 
2. Navigate to root directory 👉️
3. Use below command 
```js
amplify publish
```