node {
    stage('Checkout') {
        checkout scm
    }
    stage('Example Build') {
        echo 'Hello World'
        
    }
    stage('Example Deploy') {
            
        flyway installationName:'jenkins flyway', flywayCommand:'info',url:'jdbc:mysql://localhost:9000',locations:'./flyway',credentialsId:'',commandLineArgs:''
           
        
    }
    
}