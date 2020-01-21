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
                                notifySlack("Test Message")
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
