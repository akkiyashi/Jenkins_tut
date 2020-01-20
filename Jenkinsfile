pipeline{
        agent none 
        stages{
                stage("Output"){
                        steps{
                                echo "Hello World"
                        }
                }
                stage("Process"){
                        steps{
                                sh ps -ef
                        }
                }
        }
}
