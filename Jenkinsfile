currentBuild.displayName = "Maven-#"+currentBuild.number

pipeline{
    agent any
    stages{
        stage("Git checkout"){
          steps{
             git credentialsId: 'Github', url: 'https://github.com/rajesh9985/practice.git'
           }            
        }
        stage("Build"){  
          steps{         
            sh "mvn install"
           }
        }
    }
}
