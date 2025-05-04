pipeline{
    agent any
    tools{
        maven 'maven'
    }
   stages{
       stage('Pull src'){
           steps{
              git branch:'main', url:'https://github.com/Su-has-21/webpage.git'
           }
       }
       stage("Prep build"){
           steps{
               sh '''
                  mvn clean package
               '''
       }
     }
   }
}
