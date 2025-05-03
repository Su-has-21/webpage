pipeline{
    agent any
    tools{
        maven 'maven'
        'git'
    }
   stages{
       stage('pull src'){
           steps{
              git branch:'main', url:'https://github.com/Su-has-21/webpage.git'
           }
       }
       stage("prep build"){
           steps{
               sh '''
                  mvn clean deploy -s Settings.xml
               '''
       }
     }
   }
}
