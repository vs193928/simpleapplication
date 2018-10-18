pipeline {
    agent any

    parameters {
        booleanParam(defaultValue: true, description: '', name: 'userFlag')
    }

    stages {
        stage("foo") {
            steps {
                echo "**********flag: ${params.userFlag}"
            }     
       }
       stage("foo2") {
       steps {
                sh 'mvn clean deploy -DmuleDeploy'
            } 
    }
}
}