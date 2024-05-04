# Welcome to your CDK Go project!

This is a blank project for CDK development with Go.

The `cdk.json` file tells the CDK toolkit how to execute your app.

## Useful commands

 * `cdk deploy`      deploy this stack to your default AWS account/region
 * `cdk diff`        compare deployed stack with current state
 * `cdk synth`       emits the synthesized CloudFormation template
 * `go test`         run unit tests


# Setup 
Make aws account with the necessary cloudformation and related services + roles enabled.

# Endpoints 

# New User 
```
curl -X POST <aws_url>/register -H "Content-Type:application/json" -d '{"username":"test", "password":"test"}'
>>> Successfully registered user%   
```

# Access Token
```
curl -X POST <aws_url>/login -H "Content-Type:application/json" -d '{"username":"test", "password":"test"}'
>>> {"access_token":"xxx_xxx_xxx"}%                                                                                                       
```

# Validate Token
```
curl -X GET <aws_url>/protected -H "Content-Type:application/json" -H "Authorization:Bearer xxx-xxx-xxx"
```