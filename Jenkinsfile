currentBuild.displayName = "Maven"

pipeline{
    agent any
    stages{
        stage("Getlost"){
        steps{
            echo "Yahase nikalo"
        steps("maven_invoker invokerBuildDir: 'target/it', reportsFilenamePattern: 'target/invoker-reports/BUILD*.xml')
            sh 'mvn install'
             }
        }
    }
}
