pipeline{
        agent any
        stages{
                stage("Output"){
                        steps{
                                echo "Hello World"
                        }
                }
                if (env.BRANCH_NAME == 'master'){
                stage("Process"){
                        steps{
                                sh 'ps -ef'
                        }
                }
                }
        }
}
