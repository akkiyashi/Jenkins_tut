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
