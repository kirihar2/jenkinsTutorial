node {
    stage('Checkout') {
        checkout scm
    }
    stage('Example Build') {
        echo 'Hello World'
        
    }
   stage('test') {
    freeStyleJob('FlywayRunnerJob') {
        steps (
          flywayRunner {
            name('flyway')
            command('migrate')
            url('jdbc:mysql://mysqlserver:3306/mydb')
            locations('filesystem:$WORKSPACE/dbscripts')
            credentialsId('44620c50-1589-4617-a677-7563985e46e1')
          }
        )
    }
   }
    
}