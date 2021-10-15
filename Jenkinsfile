pipeline {
   

    triggers {
        pollSCM('H/5 * * * *')
    }

    stages {
        stage('Build') {
            steps {
                dir("spring-boot-maven-example-helloworld") {
                    sh "mvn clean package"
                }
            }
        }
    }
}
