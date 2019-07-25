node {
    stage('Checkout') {
        checkout scm
    }
    stage('Example Build') {
        echo 'Hello World'
        
    }
   stage('test') {
    steps {
        flywayrunner {name ('flyway') command ('info') url ('myDBUrl') locations ('filesystem:$WORKSPACE/main') credentialsId ('xxx there is actual value xxx') commandLineArgs ('table=myTable')}
    
    }
   }
    
}