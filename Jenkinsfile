node {
    stage('Checkout') {
        checkout scm
    }
    stage('Example Build') {
        echo 'Hello World'
        
    }
    stage('Example Deploy') {
            
         flywayrunner { 
            name('flyway') command('info') url('jdbc:h2://localhost:8082') commandLineArgs('-skipDefaultResolvers=true')
        } 
     
        
    }
    
}