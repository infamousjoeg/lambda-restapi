# lambda-restapi

An AWS Lambda-based REST API using Python + Flask routed through AWS API Gateway.

**This will be for personal use only.  This README will not apply to anyone but myself.**

## Requirements

* Python 3.8 `$ brew install python3`
* Pipenv `$ pip install pipenv --user`
* node `$ brew install node`
* serverless `$ npm install serverless --global`
* Summon ([](https://cyberark.github.io/summon))
* A Summon Provider ([](https://cyberark.github.io/summon/#providers))

## Deploy

1. Install Python dependencies in Pipenv virtual environment: `$ pipenv install`
2. Start a shell in the Pipenv virtual environment: `$ pipenv shell`
3. Create the app in Serverless ([](https://serverless.com)): `$ npx sls create -org infamousjoeg -app lambda-restapi`
4. Run `summon` to inject secret variables for AWS Access Key for deployment: `$ summon npx sls deploy`

## Remove

`$ summon npx sls remove`