node {
    stage('Checkout') {
        checkout scm
    }
    stage('Example Build') {
        echo 'Hello World'
        
    }
    freeStyleJob('FlywayDSLTest') {
     steps { 
        flywayrunner { 
            name('flyway') command('info') url('jdbc:mysql://mysqlserver:3306/mydb') commandLineArgs('-skipDefaultResolvers=true') } } }
    
}