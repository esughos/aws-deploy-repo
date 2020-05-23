pipeline {
   agent any
   stages {
      stage ('GIT Checkout') {
         steps {
        sh "export AWS_DEFAULT_REGION=us-west-2"
        sh "aws cloudformation create-stack --stack-name myteststack --template-body file://s3bucket.json --region 'us-west-2'"
 
       }
    }
  }
}
