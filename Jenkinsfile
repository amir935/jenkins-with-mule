pipeline
{ 
 agent any 
   stages{
     stage('build Application'){
     steps{
     bat 'mvn clean install'
     }
     }
     stage('munit testing'){
     steps{
     bat 'mvn test'
     }
     }
     stage('deploying mule application'){
     steps{
     bat 'mvn package deploy -DmuleDeploy'
          }
     }
  }
}
     