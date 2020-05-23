pipeline {
   agent any
   stages {
      stage ('CFT Stack Deployment') {
         steps {
        sh "export AWS_DEFAULT_REGION=us-west-2"
        sh "aws cloudformation create-stack --stack-name myteststack --template-body file://s3bucket.json --region 'us-west-2'"
 
       }
    }
  }
}
