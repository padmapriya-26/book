pipeline {
    agent {
        label 'java-slave'
    }
    stages {
        stage ('time') {
            steps {
                timeout(time:50,unit:'SECONDS') {
                    echo "+++sleeping for 50 seconds"
                    sleep 50
                }
                echo "this is the jenkinsfile"
                sh "hostname -i"
            }
        }
    }
}
