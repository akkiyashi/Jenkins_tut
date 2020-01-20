pipeline{
        agent any
        stages{
                stage("Output"){
                        steps{
                                echo "Hello World"
                        }
                }
                stage("Process"){
                        steps{
                                if(env.BRANCH_NAME == 'master') {
                                sh 'ps -ef'
                                }
                        }
                }
        }
}
