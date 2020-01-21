env.jenkins_node_custom_workspace_path = "/opt/bitnami/apps/jenkins/jenkins_home/${JOB_NAME}/workspace"
pipeline{
        agent any
        stages{
                stage("Output"){
                        steps{
                                echo "Hello World"
                        }
                }
                stage("Notify"){
                        steps{
                                slackSend color: '#BADA55', message: 'Hello, World how are you!! This your host Amrut'
                                input 'Do you approve?'
                        }
                }
                stage("Process"){
                        steps{
                                script {
                                        if(env.BRANCH_NAME == 'master') {
                                        sh 'ps -ef'
                                        }
                                }
                        }
                }
        }
}
