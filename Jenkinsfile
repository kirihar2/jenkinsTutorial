node {
    stage('Checkout') {
        checkout scm
    }
    stage('Example Build') {
        echo 'Hello World'
        
    }
    stage('Example Deploy') {
            
        //flywayrunner installationName:'jenkins flyway', flywayCommand:'info',url:'jdbc:mysql://localhost:9000',locations:'./flyway',credentialsId:'',commandLineArgs:''
          flywayrunner {
            name('flyway')
            command('migrate')
            url('jdbc:mysql://mysqlserver:3306/mydb')
            locations('filesystem:$WORKSPACE/dbscripts')
            credentialsId('44620c50-1589-4617-a677-7563985e46e1')
          }
        
    }
    
}