# AWS

## References

[ accessing your instance over ssh ] [ https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AccessingInstancesLinux.html ]

[ AWS cli howto ] [ https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-welcome.html ] 

## Private key
~/Development/aws/kh-default.pem
chmod 400 ~/Development/aws/kh-default.pem

## access to EC2
ssh -i /path/my-key-pair.pem ec2-user@ec2-198-51-100-1.compute-1.amazonaws.com

get the DNS name from here, default ubuntu username is 'ubuntu'

https://eu-west-1.console.aws.amazon.com/ec2/home?region=eu-west-1#Instances:search=i-0b86422e1f9cebff7;sort=instanceId


ssh -i ~/Development/aws/kh-default.pem ubuntu@ec2-63-35-231-236.eu-west-1.compute.amazonaws.com

## AWS CLI
https://github.com/aws/aws-cli

https://docs.aws.amazon.com/cli/latest/userguide/install-virtualenv.html

virtualenv installed in ~/Development/aws/bin

        cd bin
        source activate
        pip install --upgrade awscli
        aws --help
