# Vancy Backend Challenge

The challenge is designed to demonstrate skills required to create and advance backend services.

After this challenge you should have learned:

- Setting up a NodeJS project with typescript
- Bootrapping a web server
- Setting up an AWS Account
- Fetching Content from a S3 Bucket
- Write unit tests

At the end of the 7-Day Code Challenge, please commit and push your code to github and send the link of repo to `p.meyer@vancy.network`

💡 Make sure your commit messages are clear as well as your code.

### Step 1 - Setup

#### Project Setup

- Fork this repository
- Initialize a typescript + eslint (recommended settings for typescript) + nodejs project (Please read introduction to Typescript)
  💡 This has been done over 1 million times, the internet may help you find a good setup
- make sure that you can start a nodejs webserver (this will involve some coding)

#### AWS Setup

- Create an AWS Account
- Setup a S3 Bucket
- Upload `cuisines.json` provided with this challenge to S3 Bucket
- Setup an IAM user, create API credentials for users and store them locally into you `~/.aws/credentials` file or similar (see Documentation for AWS credentials local setuo)

💡 AWS might require you to enter a payment information for your account in order to be able to create an S3 Bucket. This should not result in actual costs for you during this challenge. Please make sure to cancel your AWS account if you don't need it anymore afterwards.

Disclaimer: valy networks UG is not covering any costs that may occur, AWS offers a 12 month free tier for the S3 Bucket at no cost.

### Step 2 - Cuisine API

The requirements for this API is the following:

- expose a REST endpoint under path `/cuisine`
- should return all available `cuisines` that are contained within the `cuisines.json` you uploaded in the setup.
- query parameters can contain a `sortBy` parameter which can either be `ASC` or `DESC`. Depending on value the list returned should be sorted alphabetically either in `ascending` or `descending` order.

### Step 3 - Test Coverage

Writing tests is an important measure to ensure that our code is working. For this challenge only unit tests are required.

- You can choose a test runner / framework of your choice.
  💡 We recommend: Mocha / SinonJS

- The tests should cover the functionality from Step 3.

- All outside services and integration points can be mocked/stubed/faked as you may need to.

- I should be able to run the tests via `npm run test`
