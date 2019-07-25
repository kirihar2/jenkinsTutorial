node {
    stage('Checkout') {
        checkout scm
    }
    stage('Example Build') {
        echo 'Hello World'
        
    }
    stage('Example Deploy') {
            
         flywayrunner commandLineArgs: '-table=myTable', credentialsId: 'xxx there is actual value xxx', flywayCommand: 'info', installationName: 'Flyway', locations: 'filesystem:$WORKSPACE/main', url: 'jdbc:mysql://mysqlserver:3306/mydb' 
        
    }
    
}