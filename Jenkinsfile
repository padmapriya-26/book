pipeline {
    agent {
        label 'java-slave'
    }
    stages {
        stage ('time') {
            steps {
                timeout(time:15,unit:'SECONDS') {
                    echo "+++sleeping for 15 seconds"
                    sleep 15
                }
                echo "this is the jenkinsfile"
                sh "hostname -i"
            }
        }
    }
}
