node {
    stage('Checkout') {
        checkout scm
    }
    stage('Example Build') {
        echo 'Hello World'
        
    }
    stage('Example Deploy') {
            
        flywayrunner installationName:'jenkins flyway', flywayCommand:'info',url:'jdbc:h2://localhost:8082',locations:'./flyway',credentialsId:'',commandLineArgs:''
           
        
    }
    
}