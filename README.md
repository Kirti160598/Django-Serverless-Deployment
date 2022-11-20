# Django-Serverless-Deployment

1. Creation of RDS MYSQL Database from AWS GUI.
2. Worked with IAMPolicy as mentioned in aws_policy.txt 
3. Installed zappa
           **pip install zappa**
    
   Zappa requires virtual environment to be initiated 
       
        python -m venv venv
       
        source venv/bin/activate
4. AWS CLI installation
       
       curl "https://s3.amazonaws.com/aws-cli/awscli-bundle.zip" -o "awscli-bundle.zip"
       unzip awscli-bundle.zip
       sudo ./awscli-bundle/install -i /usr/local/aws -b /usr/local/bin/aws
5. AWS configuration

         aws configure
      
         AWS Access Key ID [None]: <access_key>
      
         AWS Secret Access Key [None]: <secret_key>
      
         Default region name [None]: <region_name>
      
         Default output format [None]: json

6. Initialization of zappa
      
         zappa init
         
7. Deployment of application
      
        zappa deploy dev
