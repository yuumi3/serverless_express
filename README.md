# Serverless + Express study

## build

```shell
mkdir serverless_express
cd serverless_express
npx serverless create --template aws-nodejs-typescript
npm install -D serverless-offline
npm install aws-lambda serverless-http express @types/express
```

## offline dev.

```shell
npx sls offline
curl -X GET  -H 'Content-Type:application/json'  'http://localhost:3000/dev/hello
curl -X POST -H 'Content-Type:application/json'  'http://localhost:3000/dev/hello/100'
```

## deploy

```shell
npx sls deploy
```