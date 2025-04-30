pipeline {
    agent { label 'docker-agent' }  // Change to 'any' if docker-agent isn't working

    stages {
        stage('Show Info') {
            steps {
                sh '''
                echo "Name: Niyathi Vasasali"
                echo "Roll No: SE23LCSE005"
                printenv
                '''
            }
        }

        stage('Create File') {
            steps {
                sh '''
                echo "This is Job F running from a Jenkinsfile in Git." > data.txt
                cat data.txt
                '''
            }
        }
    }
}
