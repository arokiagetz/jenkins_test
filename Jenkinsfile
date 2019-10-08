#!groovy

// pipeline {
//         abcs = ['a', 'b', 'c']


//     // environment {
//     //     // DB_CLI_IMAGE='databrickscli-python:3.7.4'
//     //     // POM_ARTIFACT_ID = readMavenPom().getArtifactId()
//     //     // POM_VERSION = readMavenPom().getVersion()
//     //     // APPLICATION_NAME="${env.POM_ARTIFACT_ID}"
//     //     // JAR_VERSION = "${env.POM_VERSION}-rc${env.BUILD_NUMBER}"
//     //     // scannerHome = tool 'SonarQubeScanner'
//     // }

//     // parameters {
//     //     // string(name: 'MAVEN_REPO', description: 'Location of local repo', defaultValue: '/root/.m2/repository')
//     //     // string(name: 'MAVEN_IMAGE', description: 'Maven Version to build project', defaultValue: 'maven:3.6.2-jdk-8')
//     //     // string(name: 'JENKINS_NETWORK', defaultValue: '--network=jenkins-net', description: 'Custom network to run all container,so they can communicate with each other using service name')
//     // }

//     agent any

//     stages {

//         stage('Test 1: loop of echo statements') {
//             echo_all(abcs)
//         }
        

//         // stage('Job') {

//         //     // agent {
//         //     //     docker {
//         //     //         image "${env.AZURE_REGISTRY}/${env.DB_CLI_IMAGE}"
//         //     //         args "${params.JENKINS_NETWORK}"
//         //     //         args  "--entrypoint='' "
                    
//         //     //     }
//         //     // }

//         //     steps {
//         //         // withCredentials([usernamePassword(credentialsId: 'DATABRICK_TOKEN_DEV', passwordVariable: 'DB_TOKEN_PASSWORD', usernameVariable: 'DB_TOKEN_USER')]) {
//         //         //     sh "mkdir Hello"
//         //         //     // sh "echo 'host=${env.DATABRICKS_HOST}'>> /root/.databrickscfg"
//         //         //     // sh "echo 'token=${env.DB_TOKEN_PASSWORD}'>> /root/.databrickscfg"
//         //         //     // sh "dbfs rm dbfs:/jobs/main/${env.APPLICATION_NAME}/${env.APPLICATION_NAME}-0.0.1-SNAPSHOT-jar-with-dependencies.jar"
//         //         //     // sh "dbfs cp target/${env.APPLICATION_NAME}-0.0.1-SNAPSHOT-jar-with-dependencies.jar dbfs:/jobs/main/${env.APPLICATION_NAME}"
//         //         // }           
//         //         //sh "mkdir Hello"
//         //         sh "ls -ltr"
//         //         sh ""
//         //        // something 
//         //     }
//         // }
//     }



//     // node('master') {
//     //     stage('Test 1: loop of echo statements') {
//     //         echo_all(abcs)
//     //     }
        
//     //     stage('Test 2: loop of sh commands') {
//     //         loop_of_sh(abcs)
//     //     }
        
//     //     stage('Test 3: loop with preceding SH') {
//     //         loop_with_preceding_sh(abcs)
//     //     }
        
//     //     stage('Test 4: traditional for loop') {
//     //         traditional_int_for_loop(abcs)
//     //     }
//     // }

//     @NonCPS // has to be NonCPS or the build breaks on the call to .each
//     def echo_all(list) {
//         list.each { item ->
//             echo "Hello ${item}"
//         }
//     }

// }





//import jenkins.model.Jenkins

pipeline {
    agent any
    stages {
        stage('Preparing machines') {
            steps {
                script {
                    def machines = ['agent-windows0', 'agent-windows1', 'agent-redhat0', 'agent-redhat1']
                    //def machinePreparations = [:]

                    for (machine in machines) {
                        echo "This is printing ${machine}"
                    }
                }
            }
        }
    }
}