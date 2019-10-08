#!groovy

pipeline {

    environment {
        // DB_CLI_IMAGE='databrickscli-python:3.7.4'
        // POM_ARTIFACT_ID = readMavenPom().getArtifactId()
        // POM_VERSION = readMavenPom().getVersion()
        // APPLICATION_NAME="${env.POM_ARTIFACT_ID}"
        // JAR_VERSION = "${env.POM_VERSION}-rc${env.BUILD_NUMBER}"
        // scannerHome = tool 'SonarQubeScanner'
    }

    parameters {
        // string(name: 'MAVEN_REPO', description: 'Location of local repo', defaultValue: '/root/.m2/repository')
        // string(name: 'MAVEN_IMAGE', description: 'Maven Version to build project', defaultValue: 'maven:3.6.2-jdk-8')
        // string(name: 'JENKINS_NETWORK', defaultValue: '--network=jenkins-net', description: 'Custom network to run all container,so they can communicate with each other using service name')
    }

    agent any

    stages {
        

        stage('Job') {

            // agent {
            //     docker {
            //         image "${env.AZURE_REGISTRY}/${env.DB_CLI_IMAGE}"
            //         args "${params.JENKINS_NETWORK}"
            //         args  "--entrypoint='' "
                    
            //     }
            // }

            steps {
                // withCredentials([usernamePassword(credentialsId: 'DATABRICK_TOKEN_DEV', passwordVariable: 'DB_TOKEN_PASSWORD', usernameVariable: 'DB_TOKEN_USER')]) {
                //     sh "mkdir Hello"
                //     // sh "echo 'host=${env.DATABRICKS_HOST}'>> /root/.databrickscfg"
                //     // sh "echo 'token=${env.DB_TOKEN_PASSWORD}'>> /root/.databrickscfg"
                //     // sh "dbfs rm dbfs:/jobs/main/${env.APPLICATION_NAME}/${env.APPLICATION_NAME}-0.0.1-SNAPSHOT-jar-with-dependencies.jar"
                //     // sh "dbfs cp target/${env.APPLICATION_NAME}-0.0.1-SNAPSHOT-jar-with-dependencies.jar dbfs:/jobs/main/${env.APPLICATION_NAME}"
                // }           
                //sh "mkdir Hello"
                sh "ls -ltr"
               // something 
            }
        }
    }

}
