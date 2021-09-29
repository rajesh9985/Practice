currentBuild.displayName = "Maven"

pipeline{
    agent any
    stages{
        stage("Git checkout"){
          steps{
             git branch: 'main', credentialsId: 'Github', url: 'https://github.com/rajesh9985/practice.git'
                             }
               }
        stage("Build"){  
          steps{
                  "maven_invoker invokerBuildDir: 'target/it', reportsFilenamePattern: 'target/invoker-reports/BUILD*.xml'
            sh 'mvn install'
                     }
                 }
             }
        }
    }
}
