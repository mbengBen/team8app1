pipeline{
    agent any
        stages{
            stage('1 - action1'){
                steps{
                    checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'jenkins-access', url: 'https://github.com/mbengBen/team8app1.git']])
                }

            }
            stage('2 - action2'){
                steps{
                    sh 'df -h'
                }
            } 
            stage ('3 - action 3'){
                steps{
                    sh 'lsblk'
                }
            }
            stage ('4 - action 4'){
                steps{
                    sh 'cpu ls'
                }
            }
        }
    
}