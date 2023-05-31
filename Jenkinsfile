pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script{
                    readProp = readProperties file : 'usecase_properties/test.properties'
                    echo " Trying to Print ${readProp['a']}"
                    sh aws s3 cp test.txt s3://tdataset/

                }
            }
        }
    }
}