pipeline {
   agent any

   tools {
       maven 'maven'
       jdk 'Java'
   }
  // environment {
    //  dockerhub=credentials('dockerhub')
 //  }
  

   stage("packaging"){
      when{
             branch 'prod'
          }
          
         steps
            {

                sh 'mvn package -DskipTests'
            }
       }
   }
}
