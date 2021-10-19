# Using AWS Lambda with Node.js and serverless-http
1. Install following pakages
"aws-sdk": "^2.1007.0",
    "express": "^4.17.1",
    "serverless-http": "^2.7.0",
    "cors":"2.8.5"
2. Install The 
    - serverless-http in global scope    
        - THis is a Package that eliminates a boilerplate code for wrting the HTTP Activation for the Node.js REST APIs (http, express, KOA, ect.) 
3. create a serverless.yml file to define deployment instructions
3. finally deploy the serverless
    - Make sure that the AWS CLI from the Command line have already configured identity
        - aws configure
            - AccessKeyID:
            - SecretAccessKey:
            - region:
            - format
    - Run the following command         
        - serverless deploy
            - This command will create '.serverless' folder in the project
            - create zip package of the project
            - upload the zip on cloud

5. The Serverless for HTTP Lambda will use the 'API Gateway'
    - This will be used to manage the HTTP Method communications from CLient Apps to the Lambda using HTTP Proxy