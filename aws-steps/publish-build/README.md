### aws deploing builds

 1. manual publishing
    - create s3 bucket
    - add permissions (public get object to all)
    - upload built project files (for static content)

 2. automatic publishing
    - install serverless:
    https://www.serverless.com/framework/docs/getting-started/

    npm install -g serverless

    - install finch??? - not clear why do i need that.

      npm i serverless-finch
      or
      yarn add --dev serverless-finch

    serverless create --template aws-nodejs --path ./sl

    yarn run build
    yarn run deploy:s3

 3. [Configure CloudFront](https://youtu.be/8M_JoLh7tA4?t=2700)


 4. deploy
    - yarn install
    - yarn cloudfront:update:build:deploy

 5. Clean up infrastructure:
    - clean backet;
    - drop backet;
    - stop cloudFront;
    - drop cloudFront;
    