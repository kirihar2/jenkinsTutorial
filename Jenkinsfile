node {
    stage('Checkout') {
        checkout scm
    }
    stage('Example Build') {
        echo 'Hello World'
        
    }
   stage('test') {
      flywayrunner {
        name('flyway')
        command('info')
        url('jdbc:mysql://mysqlserver:3306/mydb')
        locations('filesystem:$WORKSPACE/dbscripts')
        credentialsId('44620c50-1589-4617-a677-7563985e46e1')
      }
   }
    
}