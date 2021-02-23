# aws-starter-pack

##Step 2 - AWS S3 Local

- Source: https://github.com/ar90n/serverless-s3-local

- Start:
    - 
    - Run `npm install`
    - Check for aws-cli `aws help`
      - Install aws-cli `sudo apt-get install awscli`
    - `mkdir ~/aws-data`
    - `touch ~/aws-data/data.csv`
    
- Config:
    -
    - Run `aws configure --profile s3local`
        - aws_access_key_id = S3RVER
        - aws_secret_access_key = S3RVER
        - aws-region = eu-west-1
    
- Run:
    -
    - `sls deploy`
    - `sls offline`
    - `aws --endpoint http://localhost:4569 s3 cp ~/aws-data/data.csv s3://thx-bucket/userdata.csv --profile s3local`
