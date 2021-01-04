# psycopg2-lambda-layer
AWS Lambda layer for psycopg2 

Forked from: https://github.com/jetbridge/psycopg2-lambda-layer

To deploy:

Change to appropriate version folder: 
```
cd 3.7
```
Build: 
```
./build.sh
```
Deploy:
```
sls deploy
```

To use in your serverless.yml:
```
functions:
  hello:
    handler: handler.hello
    layers:
      - arn:aws:lambda:us-west-2:529513974030:layer:psycopg2-py37:1
```
