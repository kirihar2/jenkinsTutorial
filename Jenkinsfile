pipeline {
    agent none
    stages {
        stage('Example Build') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Example Deploy') {
           steps {
                flywayrunner {
                    installationName: 'jenkins flyway'
                    flywayCommand: 'info'
                    url: 'jdbc:mysql://localhost:9000'
                    locations: './flyway'
                    credentailId: ''
                }
            }
        }
    }
}